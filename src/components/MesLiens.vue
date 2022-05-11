<template>
  <div class="links">
    <div class="portfolio">
      <a target="blank" href="https://lazez-bzh.netlify.app/">
        <figure>
          <img src="../assets/portfolio.png" alt="" />
          <figcaption><h4>Mon porfolio</h4></figcaption>
        </figure>
      </a>
    </div>
    <div class="other-links">
      <div class="git">
        <a target="blank" href="https://github.com/LazezBZH">
          <img src="../assets/github.png" alt="" />
        </a>
      </div>
      <div class="linkedin">
        <a target="blank" href="https://www.linkedin.com/in/benedicte-herault/">
          <img src="../assets/linkedin.png" alt="" />
        </a>
      </div>
      <div class="assetfirst">
        <a
          target="blank"
          href="https://app.assessfirst.com/_/profile/oxskit6r-benedicte-herault"
        >
          <img src="../assets/assetfirst.jpeg" alt="" />
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MesLiens",
};
</script>

<style scoped>
.links {
  width: 50%;
}
.portfolio img {
  width: 35rem;
}
.git img,
.linkedin img {
  width: 5rem;
}
.assetfirst img {
  width: 3.8rem;
}
.other-links {
  width: 60%;
  margin: 5rem auto;
  display: flex;
  justify-content: end;
}
.other-links div {
  margin: auto 1rem;
}
a {
  text-decoration: none;
  color: #d23b38;
}
h4 {
  margin: 0.5rem auto;
}
</style>
