<template>
<main class="my-8 mx-6">
  <div class="main-title">結帳</div>
    <div class="main-container">
      <div class="left-content top-content">
       <Stepper />
       <Form />  
       <Button />  
      </div>
      <Cart />
    </div> 
      
</main>

</template>


<style scoped>
main {
  padding: 1rem;
}
.main-container {
  display: flex;
  justify-content: space-between;

}
.main-title {
  position: relative;
  font-size: 24px;
  font-weight: 700;
  color: #2a2a2a;
  margin: 2rem 0 2rem 0;
}
.left-content {
    width: 50%;
  }
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