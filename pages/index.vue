<template>
  <div class="container-fluid">
    <div class="p-4 p-md-5">
      <div class="header mt-1">
        <div class="icon h1 d-block">🧬</div>
        <div
          class="title display-4 mt-5 d-block fw-bold"
          style="font-weight: 600"
        >
          Furkan Sahin
        </div>
        <div
          class="desc mt-2 col-md-8 p-0"
          style="font-size: 1.8rem; font-weight: light"
        >
          Back-end developer at Path but besides, he is proficient in modern
          javascript technologies such as Vue.js.
        </div>

        <div class="d-flex justify-content-start mt-3 h5 fw-normal">
          <a
            href="https://twitter.com/furkansahins34"
            class="text-dark text-border text-decoration-underline"
            >Twitter</a
          >
          <a
            href="https://github.com/swoorr"
            class="ml-2 text-dark text-border text-decoration-underline"
            >Github</a
          >
        </div>
      </div>

      <div class="projects mt-5 pt-3">
        <h1 class="mt-4 d-block">Projects</h1>
        <div class="row mt-4">
          <div class="col-md-4">
            <b-card title="SportsERP">
              <div class="card-body p-0">
                <p>
                  SportsERP is a web application for managing sports teams. It
                  is developing using Symfony/PHP and with many technologies.
                </p>
              </div>
            </b-card>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
};
</script>
<style>
@import url("https://fonts.googleapis.com/css2?family=Mochiy+Pop+P+One&display=swap");
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
</style>
