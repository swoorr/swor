<template>
  <b-container>
    <el-button class="mt-2"><b-link to="/">< Back</b-link></el-button>
    <el-card class="mt-2">
           <div
                slot="header"
                class="clearfix"> 
        <div class="d-flex justify-content-between">
          <h2>{{job.title}}</h2>
          <b class="fw-bold d-block mt-2 mb-n4 fw-new">
            {{
              (
                get_time_difference(new Date(job.start_date), (job.end_date != '-' ? new Date(job.end_date) : new Date())).days /
                30
              ).toFixed(2)
            }}
            Year
          </b>
        </div>
      </div>
      <div>
        <p>
          {{job.text}}
          <br />
          <div>
            <el-button v-for="n in job.tags" class="mb-2 ms-0 me-2" type="primary">{{n}}</el-button>
          </div>
        </p>
      </div>
    </el-card>
  </b-container>
</template>
<script>
import mixins from "~/mixins"
export default {
  name: "sportserp",
  mixins: [mixins],
  data: () => ({
    job:[]
  }),
  beforeMount(){
    fetch("https://createapi.app/api/app/bf4a0bef-7357-4ac8-ab2d-74b7cb753e97/"+this.$route.params.id)
    .then(response => response.json())
    .then(data => {
      this.job = data.data
      // this job tags split , 
      this.job.tags = this.job.tags.split(",")
    })
  }
}
</script>