<template>
  <div class="form_list" id="shipment">
    <h2 class="form_list_title">運送方式</h2>
    <div class="form_list_content shipment">
      <div class="content_row mb-5 py-3 active">
        <input
          type="radio"
          name="shipment"
          value="normal"
          data-price="0"
          checked
        />
        <div class="ship_descript">
          <p>標準運送</p>
          <p>約 3~7 個工作天</p>
        </div>
        <p class="ship_price">免費</p>
      </div>
      <div class="content_row py-3">
        <input type="radio" name="shipment" value="dhl" data-price="500" />
        <div class="ship_descript">
          <p class="highlight">DHL 貨運</p>
          <p>48小時內送達</p>
        </div>
        <p class="ship_price">$500</p>
      </div>
    </div>
  </div>
</template>