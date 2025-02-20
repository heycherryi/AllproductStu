<template>
    <nav class="navbar">
      <div class="nav-links">
        <button class="nav-button">Product</button>
        <button class="nav-button">Contact</button>
      </div>
    </nav>
  </template>
  
  <style>
  /* Navbar Styles */
  .navbar {
    width: 100%;
    height: 8vh;
    max-width: 100vw; /* ป้องกัน navbar เกินขอบหน้าจอ */
    background-color: #0a0a2a;
    color: white;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 15px 30px;
    position: fixed;
    top: 0;
    left: 0;
    z-index: 100;
    box-sizing: border-box; /* ทำให้ padding ไม่ดัน navbar เกิน */
  }
  
  /* กำหนดขนาดให้ navbar content */
  .logo {
    font-size: 24px;
    font-weight: bold;
    white-space: nowrap; /* ป้องกันตัวหนังสือแตกบรรทัด */
  }
  
  .nav-links {
    display: flex;
    gap: 30px; /* ✅ เพิ่มช่องว่างระหว่างปุ่มให้กว้างขึ้น */
    white-space: nowrap; /* ป้องกันปุ่มแตกบรรทัด */
  }
  
  /* ปรับขนาดปุ่มให้มีระยะห่างพอดี */
  .nav-button {
    background: none;
    border: 2px solid white;
    color: white;
    padding: 8px 20px;
    border-radius: 5px;
    cursor: pointer;
    transition: 0.3s;
    font-size: 16px;
    min-width: 100px; /* ป้องกันปุ่มเล็กเกินไป */
    text-align: center;
    border-radius: 50px; /* ✅ ทำให้เป็นปุ่มโค้ง */
  }
  
  /* Hover effect */
  .nav-button:hover {
    background-color: white;
    color: #0a0a2a;
  }
  </style>
  