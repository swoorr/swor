<template>
  <b-container>
    <b-link class="mt-2 btn btn-primary" to="/">< Back</b-link>
    <b-card class="mt-2">
      <b-card-header>
        <div class="d-flex justify-content-between">
          <h2>Sportserp</h2>
          <b class="fw-bold d-block mt-2 mb-n4 fw-new">
            {{
              (
                get_time_difference(new Date("2021-01-01"), new Date()).days /
                30
              ).toFixed(2)
            }}
            Month
          </b>
        </div>
      </b-card-header>
      <div class="card-body">
        <p>
          SportsERP is a web application for managing sports teams. It is
          developing using Symfony/PHP and with many technologies.
          <br />
          <div>
            <b-button>php</b-button>
            <b-button>symfony</b-button>
            <b-button>vue@2</b-button>
            <b-button>vue@3</b-button>
            <b-button>elastic-search</b-button>
            <b-button>rabbitmq</b-button>
          </div>
        </p>
      </div>
    </b-card>
  </b-container>
</template>
<script>
import mixins from "~/mixins";
export default {
  name: "sportserp",
  mixins: [mixins],
};
</script>