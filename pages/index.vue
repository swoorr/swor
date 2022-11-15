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
          Software developer(PHP/Symfony, Laravel and Javascript/Express) but
          besides, he is proficient in modern javascript technologies such as
          Vue.js.
        </div>

        <div class="d-flex justify-content-start mt-3 h5 fw-normal">
          <a
            href="https://superpeer.com/furkansahins34"
            target="_blank"
            class="text-dark text-border text-decoration-underline"
            >call</a
          >
          <a
            href="https://twitter.com/furkansahins34"
            target="_blank"
            class="ml-2 text-dark text-border text-decoration-underline"
            >tweets</a
          >
          <a
            href="https://github.com/swoorr"
            target="_blank"
            class="ml-2 text-dark text-border text-decoration-underline"
            >git</a
          >
          <a
            href="https://www.buymeacoffee.com/swor"
            target="_blank"
            class="ml-2 text-dark text-border text-decoration-underline"
            >buymeacoffee</a
          >
        </div>
      </div>

      <div class="projects mt-5 pt-3">
        <h1 class="mt-4 d-block">Summary (Total 7+ year)</h1>
        <div class="row mt-4">
          <div class="col-md-4 mb-2">
            <b-card>
              <b-card-title
                ><b-link to="/sportserp">⚽ SportsERP</b-link></b-card-title
              >
              <div class="card-body p-0">
                <p>
                  SportsERP is a web application for managing sports teams. It
                  is developing using Symfony/PHP and with many technologies.
                  <br />
                  <b class="fw-bold d-block mt-2 mb-n4 fw-new">
                    {{
                      (
                        get_time_difference(new Date("2021-01-01"), new Date())
                          .days / 30
                      ).toFixed(2)
                    }}
                    Month
                  </b>
                </p>
              </div>
            </b-card>
          </div>
          <div class="col-md-4 mb-2">
            <b-card title="👨🏻‍💻 Freelancer">
              <div class="card-body p-0">
                <p>
                  With PHP, AngularJS, Vue.js, Laravel, Codeigniter, Javascript
                  technologies <br />
                  <br />
                  <b class="fw-bold d-block mt-2 mb-n4 fw-new">
                    {{
                      (
                        get_time_difference(
                          new Date("2017-01-01"),
                          new Date("2021-01-01")
                        ).days /
                        30 /
                        12
                      ).toFixed(2)
                    }}
                    Year
                  </b>
                </p>
              </div>
            </b-card>
          </div>
        </div>
      </div>

      <div class="digitalgarden mt-5 pt-3">
        <h1 class="mt-4 d-block">Digital Garden</h1>
        <div class="row mt-4">
          <div class="col-md-4">
            <b-card title="📦 Selectable Date Picker">
              <div class="card-body p-0">
                <p class="mb-2">
                  Selectable Date Picker is a simple date picker component. It
                  is developed using Vue.js.
                </p>
                <span
                  class="badge badge-success"
                  style="font-family: sans-serif"
                  >development</span
                >
                <a
                  href="https://www.npmjs.com/package/@swoorr/vue-selectable-datepicker"
                  target="_blank"
                  >@swoorr/vue-selectable-datepicker</a
                >
              </div>
            </b-card>
          </div>
        </div>
      </div>
    </div>

    <div>
      <script src="https://widgets.superpeer.com/widget.js"></script>
      <script>
        window.addEventListener("load", () => {
          new Superpeer.Widget({
            embed: { type: "popup" },
            launcher: { type: "profile-avatar", options: {} },
            config: {
              username: "furkansahins34",
              serviceSlug: "getting-to-know",
            },
          });
        });
      </script>
    </div>
  </div>
</template>

<script>
import mixins from "~/mixins";
export default {
  name: "IndexPage",
  mixins: [mixins],
};
</script>