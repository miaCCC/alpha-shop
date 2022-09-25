<template>
  <main class="my-8 mx-6">
    <div class="main-title">結帳</div>
    <div class="main-container">
      <div class="left-content top-content">
        <Stepper :step="step"/>
        <Form :step="step"/>
        <div class="btn-section d-flex justify-content-between">
          <button
           :disabled="step === 1" 
           class="btn btn-pre"
           @click="previousStep">
            上一步
          </button>
          <button
           class="btn btn-next"
           @click="nextStep">
           {{step === 3 ? '送出訂單' : '下一步'}}
           </button>
        </div>
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

.btn-section {
margin-top: 50px;

}
.btn-next {
  color: white;
  background-color: #f67599;
}
.btn-next, .btn-pre {
    width: 50%;
    border-radius: 10px;
    padding: 12px 30px;
}


</style>

<script>
import Stepper from "../components/Stepper.vue";
import Form from "../components/Form.vue";
import Cart from "../components/Cart.vue";

export default {
  data() {
    return {
      step: 1
    }
  },
  components: {
    Stepper,
    Form,
    Cart,
  },
  methods: {
    nextStep() {
       if (this.step < 3) {
        this.step = this.step + 1
      }
      console.log(this.step)
    },
    previousStep() {
      if (this.step > 1) {
        this.step = this.step - 1
      }
    }
  }
};
</script>