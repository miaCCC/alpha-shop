<template>
  <section class="part part-2">
    <div class="main-title my-8">運送方式</div>

    <div class="shipment-container">
      
      <div class="shipment mt-3 d-flex">
        <input name="ta-gender" type="radio" value="standard" />
        <div class="shipment-choice">
          <div class="d-flex justify-content-between">
            <label for="">標準運送</label>
            <div class="price">免費</div>
          </div>
          <div class="time">
            <span>約3~7個工作天</span>
          </div>
        </div>
      </div>

      <div class="shipment mt-3 d-flex">
        <input name="ta-gender" type="radio" value="standard" />
        <div class="shipment-choice">
          <div class="d-flex justify-content-between">
            <label for="">DHL貨運</label>
            <div class="price">500</div>
          </div>
          <div class="time">
            <span>約3~7個工作天</span>
          </div>
        </div>
      </div>
    
    </div>
  </section>
</template>


<style scoped>
.shipment {
  position: relative;
  border: 1px solid lightgray;
  border-radius: 5px;
  padding: 1em;
  font-size: 14px;
  font-weight: 500;
  color: black
}
.shipment:hover {
  border: 1px solid black;
}
.shipment-choice {
  width: 100%;
  margin-left: 1rem;
}

</style>