<template>
  <div class="form_list" id="payment">
        <h2 class="form_list_title">付款資訊</h2>
        <div class="form_list_content payment">
          <div class="content_row name">
            <label>持卡人姓名</label><input type="text" class="content_row_input" placeholder="John Doe">
          </div>
          <div class="content_row card">
            <label>卡號</label><input type="text" class="content_row_input" placeholder="1111 2222 3333 4444">
          </div>
          <div class="content_row limit">
            <label>有效期限</label><input type="text" class="content_row_input" placeholder="MM/YY">
          </div>
          <div class="content_row code">
            <label>CVC/CCV</label><input type="text" class="content_row_input" placeholder="123">
          </div>
        </div>
      </div>
</template>