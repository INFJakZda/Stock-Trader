<template>
  <div>
    <app-stock 
      v-for="stock in stocks"
      :key="stock.id">
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
        { id: 1, name: "Google", price: 132 },
        { id: 1, name: "Tinder", price: 211 },
        { id: 1, name: "Yahoo", price: 41 }
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
