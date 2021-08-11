<template>
  <div class="container-fluid p-0 m-0">
    <ul class="col-lg-12 list-unstyled list-inline pl-5 mt-4">
      <li class="mr-5 ml-3 list-inline-item">
        <img src="../assets/Jobply.png" width="80" alt="">
        </li>
        <li class="mr-3 list-inline-item">
        <a href="#">
          Home
          </a>
        </li>
        <li class="mr-3 list-inline-item">
        <a href="#">
          Categories
        </a>
        </li>
        <li class="mr-3 list-inline-item">
        <a href="#">
          Services
        </a>
        </li>
        <li class="mr-3 list-inline-item">
        <a href="#">
          Jobs
        </a>
        </li> 
        <li class="float-right list-inline-item mr-5">
        <button class="btn btn-danger ml-5 pl-4 pr-4">Signup</button>
        </li>
    </ul>
    <pictures/>
  </div>
</template>

<script>
import pictures from './pictures'
export default {
  name: 'navbar',
  components: {
    pictures
  }
}
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;700&display=swap");
li a {
  font-family: 'DM Sans', sans-serif;
  font-size: 15px;
  font-weight: normal;
  color: #232443;
}

button {
  font-family: 'DM Sans', sans-serif;
  font-size: 12px;
  background: #212125;
  border: none;
}
</style>
