<template>
  <div>
    <app-stock 
      v-for="stock in stocks"
      :key="stock.id"
      :stock="stock">
    </app-stock>
  </div>
</template>

<script>
import Stock from './Stock.vue';

export default {
  data() {
    return {
      stocks: [
        { id: 1, name: "BMW", price: 10 },
        { id: 2, name: "Google", price: 132 },
        { id: 3, name: "Tinder", price: 211 },
        { id: 4, name: "Yahoo", price: 41 }
      ]
    }
  },
  components: {
    appStock: Stock
  }
};
</script>

<style>
</style>
