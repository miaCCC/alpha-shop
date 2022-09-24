<template>
  <section class="part part-3 d-none">
    <div class="main-title my-8">付款資訊</div>
    <div class="grid-part">
      <div class="form-row">
        <label for="">持卡人姓名</label>
        <input id="name" type="text" class="" placeholder="John Doe" />
      </div>
      <div class="form-row card-number">
        <label for="">卡號</label>
        <input
          id="card-number"
          type="text"
          class=""
          placeholder="1111 2222 3333 4444" />
      </div>

      <div class="form-row validity-period">
        <label for="">有效期限</label>
        <input id="validity-period" type="text" class="" placeholder="MM/YY" />
      </div>
      <div class="form-row cvc">
        <label for="">CVC/CCV</label>
        <input id="cvc" type="text" class="" placeholder="123" />
      </div>
    </div>
  </section>
</template>