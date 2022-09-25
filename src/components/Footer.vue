<template>
  <footer>
  <div class="footer-container">
    <div class="footer-logo d-flex align-items-center">
      <img src="https://upload.cc/i1/2022/06/19/0t6eUc.png" alt="">
    </div>

    <div class="footer-list service">
      <div class="main-title my-4">客戶服務</div>
      <ul class="service-list ">
        <li class="item">運送說明</li>
        <li class="item">退換貨相關</li>
        <li class="item">付款資訊</li>
        <li class="item">FAQ</li>
      </ul>
    </div>
    <div class="footer-list about">
      <div class="main-title my-4">關於我們</div>
      <ul class="service-list ">
        <li class="item">品牌故事</li>
        <li class="item">媒體連繫</li>
        <li class="item">付款資訊</li>
        <li class="item">Press kit</li>
      </ul>
    </div>

    <div class="footer-list information">
      <div class="main-title my-4">資訊</div>
      <ul class="service-list ">
        <li class="item">隱私權政策</li>
        <li class="item">Cookie</li>
        <li class="item">GDPR</li>
      </ul>
    </div>
    <div class="footer-list follow">
      <div class="main-title my-4">追蹤ALPHA SHOP</div>
      <ul class="footer-list service-list ">
        <li class="item">+886 02126456-789</li>
        <li class="item">
          <i class="fab fa-facebook-f"></i>
          <i class="fab fa-instagram"></i>
          <i class="fab fa-whatsapp"></i>
        </li>
      </ul>
    </div>
  </div>
</footer>
</template>

<style scoped>
  .footer-container {
    all: unset;
    margin-top: 30px;
    padding: 2rem;
    display: grid;
    grid-template-columns: 220px repeat(4, 1fr);
    background-color: #f0f0f5;
  }
</style>