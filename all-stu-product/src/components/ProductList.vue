<template>
    <section class="product-list">
      <h2 class="product-title">Product</h2>
      <div class="product-grid">
        <div v-for="product in products" :key="product.name" class="product-card">
          <img :src="product.image" :alt="product.name" class="product-image">
          <h3 class="product-name">{{ product.name }}</h3>
          <p class="product-description">{{ product.description }}</p>
        </div>
      </div>
      <div class="button-container">
        <button class="all-products-btn">All Product</button>
      </div>
    </section>
</template>

<script setup>
const products = [
  { name: "Patthumma LLM", image: "/path/to/image1.png", description: "Lorem ipsum dolor amet." },
  { name: "Abdul GI", image: "/path/to/image2.png", description: "Lorem ipsum dolor amet." },
  { name: "Sontana", image: "/path/to/image3.png", description: "Lorem ipsum dolor amet." },
];
</script>

<style scoped>
/* ✅ ทำให้ติดกับ HeroSection ไม่มีช่องว่าง */
.product-list {
  width: 100vw;
  min-height: 80vh;
  background: linear-gradient(to bottom, #e0e7ff, #ffffff);
  text-align: center;
  padding: 40px 5%;
  display: flex;
  flex-direction: column;
  justify-content: flex-start; /* ✅ ปรับให้อยู่ชิดบนสุด */
  align-items: center;
  box-sizing: border-box;
  margin: 0; /* ✅ ลบ margin ที่อาจดันให้เกิดช่องว่าง */
}

/* ✅ Grid แสดงผลแบบ Responsive */
.product-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 25px;
  width: 100%;
  max-width: 1200px;
}

/* ✅ การ์ดสินค้า */
.product-card {
  background: white;
  padding: 20px;
  border-radius: 15px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
  text-align: center;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  display: flex;
  flex-direction: column;
  align-items: center;
}

/* ✅ Hover Effect */
.product-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 6px 15px rgba(0, 0, 0, 0.2);
}

/* ✅ ปุ่ม All Product */
.button-container {
  margin-top: 40px;
}
.all-products-btn {
  padding: 12px 28px;
  font-size: 16px;
  font-weight: bold;
  border: 2px solid #6b7280;
  background: white;
  color: #374151;
  border-radius: 50px;
  cursor: pointer;
  transition: 0.3s ease;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.15);
}
.all-products-btn:hover {
  background: #6b7280;
  color: white;
}
</style>
