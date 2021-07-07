<template>
  <v-layout row wrap>
    <Stock v-for="stock in stocks" :key="stock.id" :stock="stock"></Stock>
  </v-layout>
</template>

<script>
import Stock from "./Stock.vue";

export default {
  components: { Stock },
  data() {
    return {
      stocks: [
        { id: 1, name: "BMW", price: 110 },
        { id: 2, name: "GOOGLE", price: 200 },
        { id: 3, name: "APLE", price: 280 },
        { id: 4, name: "TWITTER", price: 83 },
      ],
    };
  },
};
</script>

<style>
</style>