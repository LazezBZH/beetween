<template>
  <div class="moi2">
    <div>
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 -100 1680.75 200">
        <path
          id="vague"
          fill="none"
          stroke="transparent"
          d="M.36,90.6c44.09-46,109.57-98.57,182-88.81C257.49,11.92,271,78.85,348.25,90.6c95.57,14.54,119-81.74,230.15-85.82C683.51.93,697.28,86.67,808.54,87.61c109.2.92,119.91-81.46,229.25-86.82,134.34-6.58,155.42,100.19,279.57,89,114.46-10.31,163.52-104.74,260.11-77,37.71,10.82,87.6,58.49,102.89,77"
        />
        <text font size="35px">
          <textPath id="chemin" href="#vague" startOffset="100" fill="#d23b38">
            Je suis Bénédicte Hérault
          </textPath>
        </text>
      </svg>

      <img class="moi" alt="moi" src="../assets/moi.jpg" />
    </div>
  </div>
</template>

<script>
export default {
  name: "MoiCest",
};
</script>

<style scoped>
.moi {
  width: 12rem;
  margin: -10rem auto auto auto;
  border-radius: 50%;
  -webkit-animation: spin 300ms linear 4;
  -moz-animation: spin 300ms linear 4;
  animation: spin 300ms linear 4;
  z-index: -1;
  float: right;
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
#chemin {
  font-size: 4rem;
}
.moi2 {
  width: 60%;
  margin-top: -10rem;
  margin-left: 5rem;
}
@media (max-width: 1060px) {
  .moi {
    width: 8rem;
    margin: -7rem auto auto -7rem;
  }
}
@media (max-width: 750px) {
  .moi {
    width: 5rem;
    margin: 0rem auto auto -7rem;
  }
  #chemin {
    font-size: 6rem;
  }
}
</style>
