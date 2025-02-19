<script setup>
import Navbar from './components/Navbar.vue';
import HeroSection from './components/HeroSection.vue';
import ProductList from './components/ProductList.vue';

</script>


<template>
  <Navbar/>
  <main class="container">
    <HeroSection />

  </main>

</template>

<style scoped>
/* ✅ ทำให้ HeroSection และ ProductList ต่อกัน */
.container {
  display: flex;
  flex-direction: column;
  width: 100vw;
  overflow-x: hidden;
}
</style>