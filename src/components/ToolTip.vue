<template>
  <div :class="`tooltip ${position}`">
    <slot></slot>
    <span class="tooltip-text">
      <img :src="require(`../assets/${image}`)" alt="" /><br />{{
        content
      }}</span
    >
  </div>
</template>

<script>
export default {
  name: "ToolTip",
  props: {
    position: String,
    content: String,
    image: String,
  },
};
</script>
<style scoped>
.tooltip {
  position: relative;
  display: inline-block;
}
.tooltip .tooltip-text {
  visibility: hidden;
  width: 20rem;
  height: 15rem;
  background-color: #d23b38;
  color: #fff;
  text-align: center;
  border-radius: 6px;
  padding: 5px 0;
  position: absolute;
  z-index: 1;
  opacity: 0;
  transition: opacity 0.5s;
}

/* Tooltip top content */
.top .tooltip-text {
  bottom: 100%;
  left: 50%;
  margin-left: -10rem; /* 120/2 = 60 */
}
/* Tooltip right content */
.right .tooltip-text {
  top: -5rem;
  left: 110%;
}
/* Tooltip bottom content */
.bottom .tooltip-text {
  top: 100%;
  left: 50%;
  margin-left: -10rem; /* 120/2 = 60 */
}
/* Tooltip left content */
.left .tooltip-text {
  top: -5rem;
  right: 110%;
}
.tooltip .tooltip-text::after {
  content: "";
  position: absolute;
  border-width: 5px;
  border-style: solid;
}
/* Tooltip top arrow */
.top .tooltip-text::after {
  margin-left: -5px;
  left: 50%;
  top: 100%;
  border-color: #555 transparent transparent transparent;
}
/* Tooltip bottom arrow */
.bottom .tooltip-text::after {
  margin-left: -5px;
  bottom: 100%;
  left: 50%;
  border-color: transparent transparent #555 transparent;
}
/* Tooltip left arrow */
.left .tooltip-text::after {
  top: 50%;
  margin-top: -2rem;
  left: 100%;
  border-color: transparent transparent transparent #555;
}
/* Tooltip right arrow */
.right .tooltip-text::after {
  top: 50%;
  margin-top: -2rem;
  right: 100%;
  border-color: transparent #555 transparent transparent;
}
.tooltip:hover .tooltip-text {
  visibility: visible;
  opacity: 1;
}
.tooltip img {
  width: 10rem;
  height: 10rem;
  object-fit: contain;
}
</style>
