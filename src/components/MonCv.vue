<template>
  <div class="cv">
    <div class="image-zoom">
      <input type="checkbox" id="zoomCheck" v-model="checked" />

      <label for="zoomCheck">
        <img src="../assets/cv.png" alt="" />
      </label>
    </div>
    <button className="download">
      <a
        target="blank"
        href="https://drive.google.com/file/d/1uriO8ogWo7sQfrheJk-guhOqYHSjh-eU/view?usp=sharing"
      >
        Téléchargez PDF
      </a>
    </button>
  </div>
</template>

<script>
export default {
  name: "MonCv",
};
</script>

<style scoped>
input[type="checkbox"] {
  display: none;
}

.image-zoom img {
  width: 30%;
  transition: transform 0.25s ease;
  cursor: zoom-in;
  z-index: 99;
  padding-bottom: 5rem;
  padding-left: 2rem;
  margin: auto;
}

input[type="checkbox"]:checked ~ label > img {
  transform: scale(3) translateY(7rem);
  cursor: zoom-out;
}
.image-zoom {
  position: absolute;
  top: 5rem;
  margin-left: -5rem;
}

.cv {
  position: relative;
}
.download {
  position: absolute;
  top: 0%;
  right: 75%;
  padding: 1rem;
  border: solid 5px rgb(186, 122, 2);
  border-radius: 1rem;
  background-color: rgb(233, 220, 195);

  cursor: url("https://surlapage.fr/widget/cursors/16/1281092.gif"), default;
}
.download a {
  color: rgb(186, 122, 2);
  font-weight: bolder;
  text-decoration: none;
  cursor: url("https://surlapage.fr/widget/cursors/16/1281092.gif"), default;
}

.cv {
  width: 50%;
}
</style>
