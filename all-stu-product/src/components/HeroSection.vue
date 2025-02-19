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
    width: 100vw;  /* ✅ กว้างเต็มจอ */
    height: 60vh; /* ✅ สูงเต็มจอ */
    background: linear-gradient(to right, #4a148c, #1e3a8a);
    color: white;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: absolute; /* ✅ ชิดด้านบน */
    top: 0;
    left: 0;
    box-sizing: border-box;
    padding: 0 5vw;
  }
  
  .hero-text {
    flex: 1;
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 0 80px; /* ป้องกันการล้น */
    box-sizing: border-box;
    max-width: 80%; /* ป้องกันข้อความล้น */
    text-align: left;
  }
  
  .hero-text h1 {
    font-size: 40px;
    font-weight: bold;
    color: #34d399;
  }
  
  .hero-text p {
    margin-top: 10px;
    font-size: 23px;
    color: #d1d5db;
  }
  
  .hero-title {
    flex: 1;
    display: flex;
    justify-content: center;
    align-items: center;
    box-sizing: border-box;
    max-width: 50%;
  }
  
  .hero-title h2 {
    font-size: 80px;
    font-weight: bold;
  }
  </style>
  