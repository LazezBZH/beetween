<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
  </div>
  <p class="color">
    ColorZilla a tenté de retrouver la couleur entourant le B de votre logo, je
    ne suis pas convaincue à 100%, je lui ai pris un rdv chez un ophtalmo!
  </p>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<style scoped>
h1 {
  font-size: 4rem;
}
.color {
  width: 15rem;
  color: #d23b38;
  font-weight: bold;
  text-align: left;
  margin: -3rem auto 0 5rem;
  background-color: yellow;
  padding: 2.2rem;
  border: 1rem solid red;
  border-radius: 30% 0% 30% 50%;

  -webkit-box-shadow: 7px -5px 10px 0px #4b0082, 11px -9px 10px 0px #0000ff,
    16px -14px 10px 0px #00ff00, 20px -17px 10px 0px #ffff00,
    24px -19px 10px 0px #ff7f00, 27px -23px 10px 0px #ff0000,
    5px 5px 15px 5px rgba(0, 0, 0, 0);
  box-shadow: 7px -5px 10px 0px #4b0082, 11px -9px 10px 0px #0000ff,
    16px -14px 10px 0px #00ff00, 20px -17px 10px 0px #ffff00,
    24px -19px 10px 0px #ff7f00, 27px -23px 10px 0px #ff0000,
    5px 5px 15px 5px rgba(0, 0, 0, 0);
  transform: rotate(-20deg);
}
</style>
