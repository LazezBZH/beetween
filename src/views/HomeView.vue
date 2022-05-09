<template>
  <div class="homeAll">
    <div class="home">
      <HelloWorld msg="Hello les" />
      <img class="logoB" alt="Beetween logo" src="../assets/beetween.jpg" />
    </div>
    <div><MoiCest /></div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import MoiCest from "@/components/MoiCest.vue";

export default {
  name: "HomeView",
  components: {
    HelloWorld,
    MoiCest,
  },
};
</script>
<style scoped>
.logoB {
  width: 25%;
  margin: 8rem auto;
  position: absolute;
  left: 40%;
  -webkit-animation: spin 1s linear 5;
  -moz-animation: spin 1s linear 5;
  animation: spin 1s linear 5;
  z-index: -1;
}
@-moz-keyframes spin {
  100% {
    display: block;
    -moz-transform: rotate(360deg);
  }
}
@-webkit-keyframes spin {
  100% {
    -webkit-transform: rotate(360deg);
  }
}
@keyframes spin {
  100% {
    -webkit-transform: rotate(360deg);
    transform: rotate(360deg);
  }
}

.home {
  margin-bottom: 35rem;
}
</style>
