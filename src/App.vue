<template>
    <Navigation />
  <main class="container">
    <BillBoard />
    <ServiceList />
  </main>
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