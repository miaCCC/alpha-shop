<template>
  <div id="alpha-shop">
    <router-view />
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+TC:wght@300;400;500;700&display=swap');


/* reset css */
/* reset css */

html {
  width: 100%;
  height: 100%;
}
body {
  margin: 0;
  padding: 0;
  background-color: #fff;
  font-family: "Noto Sans TC", sans-serif; /* 設定字型 */
  font-size: 1rem;
  line-height: 1.4;
}
*,
*::before,
*::after {
  box-sizing: border-box;
}
h1,
h2,
h3,
h4,
h5,
h6,
p {
  margin: 0px;
  padding: 0px;
}
ul,
ol,
li {
  list-style-type: none; /* 拿掉前方圈圈 */
  margin: 0;
  padding: 0;
  list-style: none;
  margin: 0px;
  padding: 0px;
}
a,
a:hover,
a:focus {
  text-decoration: none;
}
img {
  display: block;
}
.btn,
button,
button:focus,
input:focus,
textarea:focus,
select,
select:focus,
a:focus {
  outline: 0px !important;
}
button {
  background-color: transparent;
  border: 0;
  cursor: pointer;
}
button[disabled] {
  pointer-events: none;
}
input {
  padding: 0;
}
input:required {
  box-shadow: none;
}
input:invalid {
  box-shadow: none;
}
</style>

<script>
import 'bootstrap'
import 'bootstrap/dist/css/bootstrap.min.css'
export default {
  name: 'alpha-shop'
}
</script>