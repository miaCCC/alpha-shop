<template>
<main class="my-8 mx-6">
  <div class="main-title my-8">結帳</div>
    <div class="main-container">
      <div class="left-content top-content">
       <Stepper />
       <Form />
       <Cart />
      </div>
    </div> 
      <Button />
</main>

</template>


<style scoped>

</style>

<script>
import Stepper from "../components/Stepper.vue";
import Form from "../components/Form.vue";
import Button from "../components/Button.vue";
import Cart from "../components/Cart.vue";

export default {
  components: {
    Stepper,
    Form,
    Button,
    Cart,
  },
};
</script>