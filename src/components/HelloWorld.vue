<template>
  <div class="hello">
    <img
      :src="pictureHover"
      @mouseover="hover = true"
      @mouseleave="hover = false"
    />
  </div>
</template>

<script>
export default {
  computed: {
    pictureHover() {
      if (this.hover === true) {
        return this.pictureGif;
      } else {
        return this.pictureStatic;
      }
    },
  },
  name: "HelloWorld",
  data() {
    return {
      pictureStatic: require("../assets/baby_alpaca.jpeg"),
      pictureGif: require("../assets/adult_alpaca.jpeg"),
      hover: false,
    };
  },
};
</script>


<style scoped>
img {
  height: 500px;
}
</style>