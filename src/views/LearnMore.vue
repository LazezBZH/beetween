<template>
  <div class="meAll">
    <h1>Vous saurez tout...ou presque!</h1>
    <div class="me"><MonCv /> <MesLiens /></div>

    <div class="teamAndMe">
      <img class="team" alt="moi" src="../assets/Beetween.gif" />
    </div>
  </div>
</template>
<script>
import MonCv from "@/components/MonCv.vue";
import MesLiens from "@/components/MesLiens.vue";

export default {
  name: "LearnMore",
  components: {
    MonCv,
    MesLiens,
  },
};
</script>
<style scoped>
.me {
  width: 100%;
  display: flex;
  flex-direction: row;
  margin: 3rem auto auto auto;
  padding-bottom: 0rem;
}
.meAll {
  margin: auto;
}
.teamAndMe {
  margin-top: -10%;
}
.team {
  width: 30%;
}
@media (max-width: 1225px) {
  .teamAndMe {
    width: 50%;
  }
  .team {
    width: 90%;
  }
}
@media (max-width: 900px) {
  .teamAndMe {
    width: 100%;
    margin: auto;
  }
  .team {
    width: 90%;
  }
}
</style>
