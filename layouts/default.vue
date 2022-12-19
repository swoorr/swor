<template>
  <div>
    <Nuxt />
  </div>
</template>
<script>
import elementUi from "element-ui"
import Vue from "vue"
Vue.use(elementUi)
//add css
import "element-ui/lib/theme-chalk/index.css"
export default {}
</script>
<style>
@import url("https://fonts.googleapis.com/css2?family=Mochiy+Pop+P+One:ital,wght@0,300;0,400;0,500;1,300;1,400;1,700&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Zilla+Slab:ital,wght@0,300;0,400;0,500;1,300;1,400;1,700&display=swap");
html,
body {
  font-family: "Zilla Slab", serif;
  color: #444;
}
.text-decoration-underline {
  text-decoration: underline;
}
.text-decoration-underline:hover {
  text-decoration: none;
}
.fw-new {
  font-family: "Mochiy Pop P One", sans-serif;
}
</style>
