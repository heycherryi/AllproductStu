<template>
    <section class="hero-section">
      <!-- ส่วนซ้าย: ข้อความ -->
      <div class="hero-text">
        <h1>Speech and Text Understanding Research Team (STU)</h1>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Facilisis penatibus sapien fusce vel curae elementum.
          Gravida quisque feugiat per bibendum integer vitae ut. Iaculis platea efficitur posuere ultricies potenti interdum.
        </p>
      </div>
  
      <!-- ส่วนขวา: STU -->
      <div class="hero-title">
        <h2>STU</h2>
      </div>
    </section>
</template>
  
<style scoped>
.hero-section {
  width: 100vw; /* ✅ กว้างเต็มจอ */
  min-height: 55vh; /* ✅ ปรับให้สูงพอดี */
  background: linear-gradient(to right, #4a148c, #1e3a8a);
  color: white;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 60px 5vw; /* ✅ ปรับ padding ให้พอดี */
  box-sizing: border-box;
  position: relative; /* ✅ ไม่ให้ทับ Navbar */
  margin-bottom: 0; /* ✅ ไม่ให้เว้นระยะด้านล่าง */
}

/* ✅ ป้องกันไม่ให้ข้อความล้น */
.hero-text {
  flex: 1;
  max-width: 45%;
  text-align: left;
}

/* ✅ หัวข้อ */
.hero-text h1 {
  font-size: 40px;
  font-weight: bold;
  color: #34d399;
}

/* ✅ คำอธิบาย */
.hero-text p {
  margin-top: 10px;
  font-size: 18px;
  color: #d1d5db;
}

/* ✅ ตำแหน่งโลโก้ STU */
.hero-title {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
  max-width: 40%;
}

/* ✅ ขนาดตัวอักษรใหญ่ขึ้น */
.hero-title h2 {
  font-size: 90px;
  font-weight: bold;
  text-transform: uppercase;
  color: white;
}

/* ✅ ปรับ Responsive สำหรับมือถือ */
@media (max-width: 768px) {
  .hero-section {
    flex-direction: column;
    text-align: center;
    min-height: 80vh;
  }
  
  .hero-text {
    max-width: 90%;
    text-align: center;
  }

  .hero-title {
    max-width: 100%;
    margin-top: 20px;
  }
}
</style>
