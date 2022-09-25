<template>
  <section class="part part-3">
    <div class="main-title my-8">付款資訊</div>
    <div class="grid-part">
      <div class="form-row">
        <label for="">持卡人姓名</label>
        <input
         v-model="cardInfo.name"
         id="name"
         type="text" 
         placeholder="John Doe" />
      </div>
      <div class="form-row card-number">
        <label for="">卡號</label>
        <input
         v-model="cardInfo.number"
         id="card-number"
         type="text"
         placeholder="1111 2222 3333 4444" />
      </div>
      <div class="form-row validity-period">
        <label for="">有效期限</label>
        <input
         v-model="cardInfo.validityPeriod"
         id="validity-period"
         type="text"
         placeholder="MM/YY" />
      </div>
      <div class="form-row cvc">
        <label for="">CVC/CCV</label>
        <input
         v-model="cardInfo.cvc"
         id="cvc"
         type="text"
         placeholder="123" />
      </div>
    </div>
  </section>
</template>

<style scoped>
input, 
select {
  padding: 0;
  width: 100%;
  border: 1px solid #4a4a4a;
  border-radius: 5px;
  font-size: 12px;
  padding: 1em;
  opacity: 0.5;
  }
label {
  display: block;
  margin-bottom: 6px;
  font-size: 12px;
  font-weight: 500;
  color: #808080;
}
.grid-part {
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  grid-gap: 0.5rem 2rem;
  margin: 5px;
}
.form-row {
    grid-column: 1 / 7;
  }
.validity-period {
    grid-column: 1 / 4;
  }
  .cvc {
    grid-column: 4 / 7;
  }
</style>

<script>
export default {
  data () {
    return {
      cardInfo: {
        number: '',
        validityPeriod: '',
        cvc: '',
      },
    }
  }
}
</script>