<template>
  <div class="right-content">
    <h3 class="my-2">購物籃</h3>
    <div 
      class="cart-container" 
      v-for="product in products"
      :key="product.id">
      <div class="product-panel d-flex">
        <img
          :src="product.image"
          alt=""
          class="product-img"/>
        <div class="product-list">
          <div class="mb-2">
            <span class="product-name">{{product.name}}</span>
          </div>
          <div class="mb-7">
            <span
              class="cursor-pointer"
              @click.stop.prevent="quantityMinus(product.id)">
              <i class="fa-solid fa-circle-minus"></i>
            </span>
            <span class="amount">{{product.quantity}}</span>
            <span 
              class="cursor-pointer"
              @click.stop.prevent="quantityPlus(product.id)">
              <i class="fa-solid fa-circle-plus"></i>
            </span>
          </div>
          <div class="product-price">
            <p>$
              <span class="price">
              {{(product.price * product.quantity).toLocaleString("en-US")}}</span>
            </p>
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
        <p>$<span class="total">{{totalPrice.toLocaleString("en-US")}}</span></p>
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

<script>
const dummyData = {
  products: [
    {
      id: 1,
      name: '破壞補釘修身牛仔褲',
      image: 'https://i.postimg.cc/BZ5YL2Bf/Block-2px.png',
      price: 3999,
      quantity: 1
    },
    {
      id: 2,
      name: '刷色直筒牛仔褲',
      image: 'https://i.postimg.cc/dQz8NvZJ/Block-2x.png',
      price: 1299,
      quantity: 1
    }
  ]
}

export default {
  data() {
    return {
      products: [],
    }
  },

  methods: {
    fetchProducts() {
      this.products = dummyData.products
    },
    quantityMinus(id) {
      this.products.filter((product) => {
        if(product.id === id && product.quantity > 0) {
          return product.quantity = product.quantity - 1
        }
      }) 
    },
    quantityPlus(id) {
      this.products.filter((product) => {
        if(product.id === id) {
          return product.quantity = product.quantity + 1
        }
      }) 

    }
  },

  computed: {
    totalPrice() {
      let total = 0
      this.products.forEach(product => {
        total += product.price * product.quantity
      })
       return total
    }

  },

  created() {
    this.fetchProducts()
  }


}
</script>
