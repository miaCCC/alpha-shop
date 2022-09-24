<template>
  <div class="right-content">
    <h3 class="my-2">購物籃</h3>
    <div class="cart-container">
      <div class="cart-panel"></div>
      <div class="product-panel product-1 d-flex">
        <img
          src="https://i.postimg.cc/BZ5YL2Bf/Block-2px.png"
          alt=""
          class="product-img"
        />
        <div class="product-list product-1 ">
          <div class="mb-2">
            <span class="product-name">破壞補釘修身牛仔褲</span>
          </div>
          <div class="mb-7">
            <span class="cursor-pointer"
              ><i class="p1 fa-solid fa-circle-minus"></i
            ></span>
            <span class="amount1">1</span>
            <span class="cursor-pointer"
              ><i class="p1 fa-solid fa-circle-plus"></i
            ></span>
          </div>
          <div class="product-price">
            <p>$<span class="price price-1">3,999</span></p>
          </div>
        </div>
      </div>
      <div class="product-panel product-2 d-flex ">
        <img
          src="https://i.postimg.cc/dQz8NvZJ/Block-2x.png"
          alt=""
          class="product-img"
        />
        <div class="product-list product-2 align-items-end">
          <div class="mb-2">
            <span class="product-name">刷色直筒牛仔褲</span>
          </div>
          <div class="mb-7">
            <span class="cursor-pointer"
              ><i class="p2 fa-solid fa-circle-minus"></i
            ></span>
            <span class="amount2">1</span>
            <span class="cursor-pointer"
              ><i class="p2 fa-solid fa-circle-plus"></i
            ></span>
          </div>
          <div class="product-price">
            <p>$<span class="price price-2">1,299</span></p>
          </div>
        </div>
      </div>
    </div>
    <div class="line"></div>
    <div class="fee d-flex justify-content-between py-3">
      <div>運費</div>
      <div class="shipment-fee bold">免費</div>
    </div>
    <div class="line"></div>
    <div class="fee d-flex justify-content-between py-3">
      <div>小計</div>
      <div>
        <p>$<span class="total">5,298</span></p>
      </div>
    </div>
  </div>
</template>

<style scoped>

.right-content {
  width: 40%;
  padding: 1.5rem;
  border: 1px solid lightgray;
  border-radius: 10px;

}
.product-panel {
  margin: 3rem 0 3rem 0;
  position: relative;

}

span {
  font-size: 14px;
  margin: 0 0 1rem 1rem;
}
  
.price {
  font-size: 14px;
  font-weight: 700;
  color: black;
}
.product-price {
  position: absolute;
  right: 0;
  top: 0
}

img {
  width: 100px;
  height: 100px;
}


i {
  color: lightgray;
  font-size: 16px;
}
  
.line {
  width: 100%;
  height: 1px;
  background-color: lightgrey;
}

</style>