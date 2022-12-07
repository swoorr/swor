<template>
  <div class="container-fluid">
    <div class="p-md-5">
      <div class="header mt-1">
        <div class="title display-4 mt-2 d-block fw-bold" style="font-weight: 600">Furkan Sahin 🧬</div>
        <div class="desc mt-2 col-md-8 p-0" style="font-size: 1.8rem; font-weight: light">
          Software developer (PHP/Symfony, Laravel and Javascript/Express) but besides, he is proficient in modern javascript technologies
          such as Vuejs, Reactjs.
        </div>

        <div class="d-flex justify-content-start mt-3 h5 fw-normal">
          <el-button type="primary" plain onClick=" window.open('https://superpeer.com/furkansahins34');">
            <i class="el-icon-share"></i>
            call</el-button
          >
          <el-button type="warning" plain onClick=" window.open('https://twitter.com/furkansahins34');">
            <i class="el-icon-postcard"></i>
            tweets</el-button
          >
          <el-button type="info" plain onClick=" window.open('https://github.com/swoorr');">
            <i class="el-icon-finished"></i>
            github</el-button
          >
          <el-button type="dark" plain onClick=" window.open('https://buymeacoffee.com/swor');">
            <i class="el-icon-coffee-cup"></i>
            coffee</el-button
          >
        </div>
      </div>

      <div class="projects mt-2 pt-3">
        <h1 class="mt-4 d-block">Summary (Total 7+ year)</h1>
        <div class="row mt-4">
          <div class="col-md-4 mb-2">
            <el-card shadow="always">
              <div slot="header" class="clearfix" style="cursor: pointer">
                <b-link
                  to="/sportserp"
                  onmouseover="this.style.color='orange';"
                  onmouseout="this.style.color='#333';"
                  style="color: #333; text-decoration: none"
                  >⚽ SportsERP</b-link
                >
                <div class="float-end">
                  <b class="fw-bold d-block">
                    {{ (get_time_difference(new Date("2021-01-01"), new Date()).days / 30).toFixed(2) }}
                    Month
                  </b>
                </div>
              </div>
              <p>
                SportsERP is a web application for managing sports teams. It is developing using Symfony/PHP and with many technologies.
              </p>
            </el-card>
          </div>
          <div class="col-md-4 mb-2">
            <el-card shadow="always">
              <div slot="header" class="clearfix" style="cursor: pointer">
                <b-link
                  onmouseover="this.style.color='orange';"
                  onmouseout="this.style.color='#333';"
                  style="color: #333; text-decoration: none"
                  >👨🏻‍💻 Freelancer</b-link
                >
                <div class="float-end">
                  <b class="fw-bold d-block">
                    {{ (get_time_difference(new Date("2017-01-01"), new Date("2021-01-01")).days / 30 / 12).toFixed(2) }}
                    Year
                  </b>
                </div>
              </div>
              <p>With PHP, AngularJS, Vue.js, Laravel, Codeigniter, Javascript technologies</p>
            </el-card>
          </div>
        </div>
      </div>

      <div class="digitalgarden mt-2 pt-3">
        <h1 class="mt-4 d-block">Digital Garden</h1>
        <div class="row mt-4">
          <div class="col-md-4">
            <el-card shadow="always">
              <div
                slot="header"
                class="clearfix"
                style="cursor: pointer"
                onmouseover="this.style.color='orange';"
                onmouseout="this.style.color='';"
                onClick="window.open('https://www.npmjs.com/package/@swoorr/vue-selectable-datepicker')"
              >
                📦 Selectable Date Picker
              </div>
              <div class="card-body p-0">
                <p class="mb-2">Selectable Date Picker is a simple date picker component. It is developed using Vue.js.</p>
                <el-badge class="item">
                  <el-button type="warning" plain size="small">development</el-button>
                </el-badge>
              </div>
            </el-card>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import elementUi from "element-ui"
import Vue from "vue"
Vue.use(elementUi)
//add css
import "element-ui/lib/theme-chalk/index.css"
import mixins from "~/mixins"
export default {
  name: "IndexPage",
  mixins: [mixins],
}
</script>