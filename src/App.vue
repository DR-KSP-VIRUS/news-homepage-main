<template>
    <Navigation />
  <div class="container">
    <BillBoard />
    <ServiceList />
  </div>
</template>

<script setup>
  import Navigation from './components/Navigation.vue';
  import BillBoard from './components/BillBoard.vue';
  import ServiceList from './components/ServiceList.vue'
</script>

<style scoped>
  .container {
    padding: 0 0rem;
  }
</style>