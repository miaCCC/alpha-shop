<template>

  <section class="part part-1">
    <div class="main-title">寄送地址</div>
    <div class="grid-part">
      <div class="form-row title">
        <label>稱謂</label>
        <select
         v-model="userInfo.type" 
         name="type"
         id="type"
         required>
          <option value="mr" selected>先生</option>
          <option value="ms">小姐</option>
        </select>
      </div>
      <div class="form-row name">
        <label for="">姓名</label>
        <input
         v-model="userInfo.name" 
         id="name" 
         type="text" 
         placeholder="請輸入姓名" />
      </div>
      <div class="form-row phone">
        <label for="">電話</label>
        <input
          v-model="userInfo.phone" 
          id="phone"
          type="text"
          placeholder="請輸入行動電話" />
      </div>
      <div class="form-row email">
        <label for="">Email</label>
        <input
         v-model="userInfo.email" 
         id="email"
         type="text"
         placeholder="請輸入電子郵件" />
      </div>
      <div class="form-row city">
        <label>縣市</label>
        <select
         v-model="userInfo.city" 
         name="type"
         id="type"
         required>
          <option value="city" disabled selected>請選擇縣市</option>
          <option value="tp">台北市</option>
          <option value="ntp">新北市</option>
        </select>
      </div>
      <div class="form-row adress">
        <label for="">地址</label>
        <input
         v-model="userInfo.adress" 
         id="adress"
         type="text" 
         placeholder="請輸入地址" />
      </div>
    </div>
  </section>
</template>

<style scoped>

.form-row {
  margin-bottom: 0.5rem;
}
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
.title {
  grid-column: 1 / 3;
}
.name {
  grid-column: 3 / 7;
}
</style>


<script>
export default {
  data () {
    return {
      userInfo: {
        title: '',
        name: '',
        phone: '',
        email: '',
        address: '',
        city: '',
      },
    }
  },



  created() {
    this.getUserInfo()
  }
}
</script>