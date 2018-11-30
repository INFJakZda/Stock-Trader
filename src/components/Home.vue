<template>
  <div>
    <h1>Trade or View your portfolio!</h1>
    <hr>
    <h5>You may Save & Load your data</h5>
    <hr>
    <h5>Click on 'End Day' to begin a New Day!</h5>
    <hr>
    Your Funds: {{ funds | currency }}
  </div>
</template>

<script>
export default {
  computed: {
    funds() {
      return this.$store.getters.funds;
    }
  }
};
</script>

<style>
</style>
