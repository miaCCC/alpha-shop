<template>
   <div class="form_list " id="address">
        <h3 class="form_list_title">寄送地址</h3>
        <div class="form_list_content address">
          <div class="content_row title">
            <label>稱謂</label>
            <div class="select-wrapper">
              <select name="customer-title" class="content_row_select" required="">
                <option value="">先生</option>
                <option value="">小姐</option>
              </select>
            </div>
          </div>
          <div class="content_row name">
            <label>姓名</label><input type="text" class="content_row_input" placeholder="請輸入姓名">
          </div>
          <div class="content_row phone">
            <label>電話</label><input type="text" class="content_row_input" placeholder="請輸入行動電話">
          </div>
          <div class="content_row Email">
            <label>Email</label><input type="text" class="content_row_input" placeholder="請輸入Email">
          </div>
          <div class="content_row city">
            <label>縣市</label>
            <div class="select-wrapper">
              <select name="deliver_place" class="content_row_select" id="ship-city-select" required="">
                <!--  render city -->
              </select>
            </div>
          </div>
          <div class="content_row address">
            <label>地址</label><input type="text" class="content_row_input" placeholder="請輸入地址">
          </div>
        </div>
      </div>
</template>