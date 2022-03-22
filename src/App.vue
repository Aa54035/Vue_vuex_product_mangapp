<template>
  <div id="app">
    <product-list-one :products="products"></product-list-one>
    <product-list-two :products="products"></product-list-two>
  </div>
</template>

<script>
import productListOneVue from "./Components/product-list-one.vue";
import productListTwoVue from "./Components/product-list-two.vue";

export default {
  name: "app",
  components: {
    "product-list-one": productListOneVue,
    "product-list-two": productListTwoVue,
  },
  data() {
    return {
      products: [
        { name: "Banana", price: 50 },
        { name: "Apple", price: 100 },
        { name: "Television set", price: 60000 },
        { name: "Mobile phone ", price: 15500 },
        { name: "Laptops ", price: 50000 },
      ],
    };
  },
};
</script>

<style  >
body {
  font-family: "Redressed", cursive;
  font-size: 40px;
}
</style>
