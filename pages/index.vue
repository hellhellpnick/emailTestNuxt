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
        orderId: "#1234",
        orderDate: new Date().toLocaleDateString(),
        orderName: "Alex",
        orderPhone: "+38 098 131 23 17",
        orderEmail: "hell@gmail.com",
        orderComment: "I really want to buy this",
        orderCountry: "Ukraine",
        orderCity: "Kyiv",
        orderPostCode: "42300",
        orderStreet: "Street",
        orderHouse: "49",
        orderApartment: "53",
        orderPayment: "Pay",
        listItems: [
          {
            color: "white, red, blue",
            link: "http://shemax.coi.ua/catalog/dustcollector/manikyurnaya-vytyazhka-style-pro-shemax",
            title: "Професійна настільна витяжка — Style PRO",
            count: 3,
            price: 350,
          },
          {
            color: "yellow, red",
            link: "http://shemax.coi.ua/catalog/accessories/fartuk-Sport_SheMax",
            title: "Фартух — Sport SheMax",
            count: 2,
            price: 75,
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
      try {
        await axios.post("/mail/send", {
          config: "order",
          subject: "Order form - reddytec",
          html: this.$refs.table.$el.outerHTML,
        });
      } catch (e) {}
    },
  },
  components: { TableEmail },
};
</script>