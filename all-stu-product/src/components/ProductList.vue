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
  /* ✅ ทำให้พื้นหลังเต็มจอ */
  .product-list {
    width: 100vw; 
    min-height: 100vh; /* ✅ ขยายพื้นหลังให้เต็ม */
    background: linear-gradient(to bottom, #f5f5f5, white);
    text-align: center;
    padding: 60px 5%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    box-sizing: border-box;
    position: relative; /* ✅ ป้องกันพื้นหลังล้น */
    overflow: hidden;
  }
  
  /* ✅ ปรับขนาดของหัวข้อ */
  .product-title {
    font-size: 32px;
    font-weight: bold;
    color: #374151;
    margin-bottom: 30px;
  }
  
  /* ✅ ปรับให้ grid แสดงสินค้าเต็มที่ */
  .product-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); /* ✅ ปรับให้ขยายเต็ม */
    gap: 24px;
    width: 100%;
    max-width: 1600px; /* ✅ ขยายพื้นที่ให้กว้างขึ้น */
  }
  
  /* ✅ ทำให้กล่องสินค้าไม่แคบเกินไป */
  .product-card {
    background: white;
    padding: 24px;
    border-radius: 12px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    text-align: center;
    width: 100%;
  }
  
  /* ✅ ปรับขนาดรูปภาพสินค้า */
  .product-image {
    width: 120px;
    height: 120px;
    object-fit: contain;
    margin-bottom: 15px;
  }
  
  /* ✅ ปรับขนาดตัวอักษรให้ชัดขึ้น */
  .product-name {
    font-size: 20px;
    font-weight: bold;
    color: #1f2937;
  }
  
  .product-description {
    font-size: 16px;
    color: #6b7280;
    margin-top: 8px;
  }
  
  /* ✅ ปรับให้ปุ่มอยู่ตรงกลาง */
  .button-container {
    display: flex;
    justify-content: center;
    width: 100%;
    margin-top: 30px;
  }
  
  /* ✅ ปรับปุ่มให้เด่นขึ้น */
  .all-products-btn {
    padding: 12px 24px;
    font-size: 18px;
    border: 2px solid #6b7280;
    background: transparent;
    color: #374151;
    border-radius: 8px;
    cursor: pointer;
    transition: 0.3s;
  }
  
  .all-products-btn:hover {
    background: #6b7280;
    color: white;
  }
  </style>
  