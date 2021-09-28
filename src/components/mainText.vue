<template>
<div class="container-fluid col col-lg-4 ml-5 pl-3 p-0">
<h1 class="mt-5">
  <b>Find & Apply For<br>Your Dream Job</b>
  </h1>
  <p class="text-justify mr-5 mt-1">The website is chockablock with useful features, allowing you to efficiently search and apply for roles across all sectors, experience levels and locations.</p>
  <buttons/>
</div>
  
</template>

<script>
import buttons from './buttons.vue'

export default {
  name: 'mainText',
  components: {
    buttons
  }
}
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;700&display=swap");

h1 b {
   font-family: 'DM Sans', sans-serif;
  font-weight: bold;
  font-size: 48px;
  line-height: 65px;
}

</style>
