<template>
   <div class="btn-section d-flex justify-content-between">
    <button disabled class="btn btn-pre">上一步</button>
    <button class="btn btn-next">下一步</button>
  </div>
</template>

<style scoped>

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