<template>
  <div id="step-control" class="stepper-panel">
    <div class="stepper-container">
      <div class="step active" 
        :class="{ checked: step > 1 }">
        <div class="circle-container one"></div>
        <p class="step-title">寄送地址</p>
      </div>

      <div class="step"
       :class="{ active: step === 2, checked: step > 2 }">
        <div class="circle-container two"></div>
        <span class="connect-line"></span>
        <p class="step-title">運送方式</p>
      </div>
      <div class="step"
       :class="{ active: step === 3 }">
        <div class="circle-container three"></div>
        <span class="connect-line"></span>
        <p class="step-title">付款資訊</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.stepper-container {
  width: 100%;
  display: flex;
  justify-content: space-between;
}

.step {
  display: flex;
  align-items: center;
  position: relative;
  text-align: center;
  font-size: 16px;
  font-weight: 700;
  color: lightgray;
}
.step-title {
  margin-left: 1rem;
}
.circle-container {
    padding-top: 3px;
    height: 36px;
    width: 36px;
    background-color: #ffffff;
    border-radius: 50%;
    color: #2a2a2a;
    border: 2px solid lightgray;
}

.connect-line {
  position: absolute;
  top: 18px;
  right: 110%;
  display: block;
  width: 70px;
  height: 2px;
  background-color: lightgray;
}
.one::after {
  content: '1';
}
.two::after {
  content: '2';
}
.three::after {
  content: '3';
}
.checked .circle-container::after {
  content: '\2714';
}
.checked .circle-container,
.active .circle-container {
    background-color: #2a2a2a;
    color: #ffffff;
    border: 2px solid #2a2a2a;
    }

</style>

<script>

export default {
  props: {
    step: {
      type: Number,
      required: true
    }
  },

}
</script>
