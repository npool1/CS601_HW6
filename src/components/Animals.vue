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
        return this.pictureAdult;
      } else {
        return this.pictureBaby;
      }
    },
  },
  props: ["imgName"],
  name: "HelloWorld",
  data() {
    return {
      pictureAdult: require("../assets/adult_" + this.imgName),
      pictureBaby: require("../assets/baby_" + this.imgName),
      hover: false,
    };
  },
};
</script>


<style scoped>
img {
  border-radius: 30px;
  width: 50%;
  height: auto;
}
</style>