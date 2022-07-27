<template>
  <form
    method="POST"
    @submit="submitForm"
  >
    <h2>Test form send template email</h2>
    <div
      v-for="(item, index) in order.listItems"
      :key="index"
      style="display: flex; flex-direction: row;"
    >
      <p style="margin-right: 10px">{{item.color}}</p>
      <p style="margin-right: 10px">{{item.link}}</p>
      <p style="margin-right: 10px">{{item.count}}</p>
      <p style="margin-right: 10px">{{item.price}}</p>
    </div>
    <button
      type="button"
      @click="addItem"
    >Add item</button>
    <button type="submit">Send data</button>
    <div style="display: none">
      <TableEmail
        ref='table'
        :order="order"
      />
    </div>
  </form>
</template>
<script>
import axios from "axios";
import TableEmail from "./../components/TableEmail.vue";
export default {
  data() {
    return {
      el: "ok",
      order: {
        orderId: 1,
        orderDate: new Date().toLocaleDateString(),
        orderStatus: "now",
        orderName: "Alex",
        orderPhone: "+38 000 00 00 000",
        orderEmail: "hell@gmail.com",
        orderComment: "desc",
        orderCountry: "ua",
        orderCity: "Poltava",
        orderPostCode: "39600",
        orderStreet: "a",
        orderHouse: "49",
        orderFlat: "1",
        orderPayment: "now",
        listItems: [
          {
            color: "white",
            link: "asdad",
            count: 1,
            price: 50,
          },
        ],
      },
    };
  },
  methods: {
    addItem() {
      this.order.listItems.push({
        color: "red",
        link: "zxc",
        count: 1,
        price: 20,
      });
    },
    async submitForm(e) {
      e.preventDefault();
      var myHTML = "<div><h1>Jimbo.</h1>\n<p>That's what she said</p></div>";
      var strippedHtml = myHTML.replace(/<[^>]+>/g, "");
      // Jimbo.
      // That's what she said
      console.log(strippedHtml);
      try {
        await axios.post("/mail/send", {
          config: "order",
          subject: "Order form - reddytec",
          html: this.$refs.table.$el.outerHTML,
        });
      } catch (e) {
        console.log(e);
      }
    },
  },
  components: { TableEmail },
};
</script>