<template>
  <div class="container-fluid p-0 m-0">
    <div class="row">
    <mainText/>
    <div class="col-lg-1 ml-5 pl-5 mt-5">
    <img src="../assets/J.png" class="mt-5 ml-5" width="110" alt="">
  </div>

  <div class="col-lg-4">
    <img src="../assets/woman.png" width="" class="" alt="">
  </div>

  <div class="col-lg-1 mr-5 mt-5 pt-5">
    <img src="../assets/B.png" class="mt-5" width="120" alt="">
  </div>
  </div>

  <div class="container-fluid second-section col-lg-12">
      <h2 class="ml-4 pl-3 pt-5">
      <b>Recent Searches</b>
      </h2>
<div class="card-container row container-fluid pt-3 ml-4">
  <div class="col-lg-2 card bg-white border border-primary rounded mr-4" v-for="(obj, key) in cardJSON" :key="key">
    <div class="d-inline pt-3 pl-3">
      <img src="../assets/chrome.png" class="pt-3" alt="" width="40">
      <span class="pl-3">
        <b>{{ obj.name }} </b><br>
        <h6 class="margin-top-minus ml-5 pl-2">{{ obj.rate }} </h6></span>
      </div>
      <div>
        <span class="pl-3 mt-3">
        <b>{{ obj.role }}</b>
        </span>
        <p class="pl-3 location">{{ obj.availability }}</p>
        </div>
        <div class="d-inline pl-3 pb-4">
          <h5 class="badge badge-danger mr-2 pt-1 pr-2 pl-2 pb-1">Full-time</h5>
          <h5 class="badge badge-danger pt-1 pr-2 pl-2 pb-1">Anywhere</h5>
          </div>
          </div>
        </div>
    </div>
  </div>
</template>

<script>
import mainText from './mainText.vue'
export default {
  name: 'pictures',
  components: {
    mainText
  },

  data: () => ({
    cardJSON: [
      {
        // image: '<img src="../assets/chrome.png" class="mt-3" width="40" alt="">',
        name: 'Chrome',
        rate: '10k-20k',
        role: 'Product Manager',
        availability: 'Full Time - New york city'
      },
      {
        // image: '<img src="../assets/slack.png" class="mt-3" width="40" alt="">',
        name: 'Slack',
        rate: '15k-30k',
        role: 'Software Engineer',
        availability: 'Part Time - Canada'
      },
      {
        // image: '<img src="../assets/Twitter.png" class="mt-3" width="40" alt="">',
        name: 'Twitter',
        rate: '25k-30k',
        role: 'Android Developer',
        availability: 'Full Time - Australia'
      },
      {
        // image: '<img src="../assets/linkedin.png" class="mt-3" width="40" alt="">',
        name: 'LinkedIn',
        rate: '35k-50k',
        role: 'Frontend Developer',
        availability: 'Full Time - China'
      },
      {
        // image: '<img src="../assets/linkedin.png" class="mt-3" width="40" alt="">',
        name: 'Facebook',
        rate: '35k-60k',
        role: 'Backend Developer',
        availability: 'Part Time - Japan'
      }
    ]
  })
}
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;700&display=swap");

.second-section {
  background-image: url("../assets/bg2.png");
  width: 1500 !important;
  height: 400px;
}

h3 {
  font-family: 'DM Sans', sans-serif;
  color: #212125;
  font-size: 20px;
}

.margin-top-minus {
  font-family: 'DM Sans', sans-serif;
  font-size: 15px;
  margin-top: -15px;
}

.location {
  font-family: 'DM Sans', sans-serif;
  color: #212125;
  font-size: 12px;
}
</style>
