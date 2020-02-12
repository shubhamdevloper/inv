<template>
  <div>
    <hnavbar></hnavbar>
    <div class="background-img">
    </div>
  </div>
</template>

<script>
import Hnavbar from '../components/Hnavbar.vue'
export default {
  name: 'home',
  components: {
    'hnavbar': Hnavbar
  }
}
</script>
<style lang="scss">
body{
    margin:0px;
}
.background-img {
  background-image: url("../assets/bg-image.jpg");
  background-repeat: repeat-x;
  animation: slideleft 40000s infinite linear;
  -webkit-animation: slideleft 40000s infinite linear;
  background-size: cover;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  background-attachment: fixed;
  position: relative;
  min-height: 100vh;
}
</style>
