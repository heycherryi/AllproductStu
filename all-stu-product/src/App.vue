<script setup>
import Navbar from './components/Navbar.vue';
import HeroSection from './components/HeroSection.vue';
import ProductList from './components/ProductList.vue';
</script>

<template>
  <Navbar />
  <main class="container">
    <HeroSection />
    <ProductList />
  </main>
</template>

<style scoped>
/* ✅ จัดให้ HeroSection & ProductList ต่อกัน */
.container {
  display: flex;
  flex-direction: column;
  width: 100vw;
  overflow-x: hidden;
  margin: 0;
  padding: 0;
}

/* ✅ ลบช่องว่างที่ไม่จำเป็น */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
