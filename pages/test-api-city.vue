<template>
  <div>
    <baseSelect
      @update:modelValue="$data[selectCounty.field] = $event"
      :modelValue="$data[selectCounty.field]"
      :index="-1"
      :select="selectCounty"
      :className="'personal-office__form-select'"
    />
    <baseSelect
      @update:modelValue="$data[selectCity.field] = $event"
      :modelValue="$data[selectCity.field]"
      :index="2"
      :select="selectCity"
      :className="'personal-office__form-select'"
    />
  </div>
</template>
<script>
import BaseSelect from "~/components/BaseSelect.vue";
export default {
  data() {
    return {
      apiPopulation: [],
      fieldCountry: "",
      fieldCity: "",
      selectCounty: {
        title: "country",
        listOptions: [],
        field: "fieldCountry",
      },
      selectCity: {
        title: "city",
        listOptions: [],
        field: "fieldCity",
      },
    };
  },
  async fetch() {
    let response = await fetch(
      "https://countriesnow.space/api/v0.1/countries/population/cities"
    );
    if (response.ok) {
      let json = await response.json();
      this.apiPopulation = json.data;
      json.data.forEach((item) => {
        const checkCounty = this.selectCounty.listOptions.find(
          (el) => el == item.country
        );
        if (!checkCounty) {
          this.selectCounty.listOptions = [
            ...this.selectCounty.listOptions,
            item.country,
          ];
        }
      });
    } else {
    }
  },
  watch: {
    async fieldCountry(newValue) {
      if (newValue.length) {
        const options = {
          method: "POST",
          body: JSON.stringify({ country: newValue }),
        };
        let response = await fetch(
          "https://countriesnow.space/api/v0.1/countries/cities",
          options
        );
        if (response.ok) {
          let json = await response.json();
          json.data.forEach((item) => {
            this.selectCounty.listOptions.push(item.country);
          });
        }
      } else {
        this.selectCity.listOptions = [];
      }
    },
  },
  components: { BaseSelect },

  async mounted() {
    const options = {
      method: "GET",
      headers: {
        "X-CSCAPI-KEY":
          "Z1Uwc0Z6WGhvZ05MT3VvRzdpQzNEZEhhR3RsZWpLWlRma0pzOU82aA==",
      },
    };

    fetch("https://api.countrystatecity.in/v1/countries", options)
      .then((response) => response.json())
      .then((response) => console.log(response))
      .catch((err) => console.error(err));
  },
};
</script>