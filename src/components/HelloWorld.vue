<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
  </div>
  <p class="color">
    ColorZilla a tenté de retrouver la couleur entourant le B de votre logo, je
    ne suis pas convaincue à 100%, je lui ai pris un rdv chez un ophtalmo!
  </p>
  <img class="poppins" src="@/assets/poppins.png" alt="" />
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
.poppins {
  float: right;
  margin-top: -15%;
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
@media (max-width: 1300px) {
  h1 {
    font-size: 2rem;
  }
  .color {
    width: 10rem;
    font-size: 0.7rem;
    padding: 1rem 1rem 1rem 1.5rem;
    margin: 0rem auto 0 5rem;
  }
}
@media (max-width: 1060px) {
  .poppins {
    width: 35%;
  }
}
@media (max-width: 820px) {
  h1 {
    font-size: 2rem;
  }
  .color {
    width: 8rem;
    font-size: 0.7rem;
    padding: 0.5rem 0.5rem 0.5rem 2rem;
    margin: 0rem auto 0 5rem;
  }
}
@media (max-width: 750px) {
  h1 {
    margin-top: 6rem;
  }
  .color {
    width: 15rem;
    font-size: 0.7rem;
    padding: 0.5rem 0.5rem 0.5rem 2rem;
    margin: -9rem auto 0 1rem;
    transform: none;
  }
}
@media (max-width: 425px) {
  h1 {
    margin-top: 2rem;
  }
  .color {
    width: 4.3rem;
    position: absolute;
    top: 2%;
    right: 2%;
    margin: 0;
    padding: 0.2rem;
    border-radius: 0% 30% 50% 30%;
  }
  .poppins {
    margin-top: -15%;
  }
}
</style>
