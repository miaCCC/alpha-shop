<template>

  <div class="container mt-5">
    <h3 class="main_title mb-5 mx-3">結帳</h3>
    <main>
    <section class="customer_info">
    
      <Stepper />
      <Form />
      <Button />
    
    </section>

    <section class="cart">
      <Cart />

    </section>
    </main>
  </div>

</template>


<style scoped>
main {
  display: flex;
  justify-content: space-between;
  height: 90%;
  width: 100%;
  margin: auto;
}
</style>

<script>
import Stepper from '../components/Stepper.vue'
import Form from '../components/Form.vue'
import Button from '../components/Button.vue'
import Cart from '../components/Cart.vue'


export default {
  components: {
    Stepper,
    Form,
    Button,
    Cart,
  },
  }

  </script>