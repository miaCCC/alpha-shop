<template>
    <header>
    <nav class="nav  py-3">
  
      <ul class="nav-list">
        <li class="nav-item">
          <a class="nav-link" href="#">男裝 </a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">女裝</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">最新消息</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">客制商品</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">聯絡我們</a>
        </li>
        <li class="navbar-icons ">
          <a href="#" class="icon search">
            <i class="fa-solid fa-magnifying-glass"></i>
          </a>
          <a href="#" class="icon cart">
            <i class="fa-solid fa-cart-shopping"></i>
          </a>
          <a href="#" class="dark-mode icon moon">
            <i class="fa-solid fa-moon"></i>
          </a>
        </li>
      </ul>
      <a href="#" class="navbar-brand">
        <img
          src="https://upload.cc/i1/2022/06/19/0t6eUc.png"
          alt=""
          class="navbar-brand-logo"
        />
      </a>
      <!--手機版不顯示-->
      <li class="navbar-icons-875 d-none">
        <a href="#" class="icon search">
          <i class="fa-solid fa-magnifying-glass"></i>
        </a>
        <a href="#" class="icon cart">
          <i class="fa-solid fa-cart-shopping"></i>
        </a>
        <a href="#" class="dark-mode icon moon">
          <i class="fa-solid fa-moon"></i>
        </a>
      </li>
    </nav>
  </header>
</template>

<style scoped>
header {
  position: relative;
  height: 90px;
  text-align: center;
  /* 陰影 */
  -webkit-box-shadow: 0px 2px 12px 0px rgba(0, 0, 0, 0.1);
  -moz-box-shadow: 0px 2px 12px 0px rgba(0, 0, 0, 0.1);
  box-shadow: 0px 2px 12px 0px rgba(0, 0, 0, 0.1);
}
.nav {
    position: relative;
    all: unset;
    display: grid;
    grid-template-columns: 1fr auto minmax(100px, 1fr);
    align-items: center;
    grid-gap: 2rem;
  }
 .nav-list {
    all: unset;
    padding-left: 20px;
    display: grid;
    grid-auto-flow: column;
    grid-gap: 0.5rem;
  }
  .navbar-icons {
    position: absolute;
    right: 1rem;
    top: 2rem
  }
  .navbar-icons-875 {
    display: block;
    position: absolute;
    right: 0;
  }
.icon {
  padding: 0.5rem;
}
.nav-item {
  margin: 1rem 0;
}
</style>