<template>
  <div id="home">
    <waves />
    <div class="">
      <img src="Waveslogo.png" fluid alt="Responsive image" class="logo floating">

  </div>
  </div>
</template>

<script>
  // import * as THREE from 'three'
  export default {
    name: 'Home',

    components: {
      Waves: () => import('@/components/home/Waves')
    }
  }
</script>

<style scoped>

.logo {
  position: absolute;
  top: 5%;
  right: 10%;
  height: auto;
  width: 80%;
  float: center;
  z-index: 2;

}

.floating {  
    animation-name: floating;
    animation-duration: 3s;
    animation-iteration-count: infinite;
    animation-timing-function: ease-in-out;
}

@keyframes floating {
    from { transform: translate(0,  0px); }
    50%  { transform: translate(0, 20px); }
    to   { transform: translate(0, -0px); }    
}
</style>
