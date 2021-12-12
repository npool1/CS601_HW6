<template>
  <div id="app">
    <animals label="animals" img-name="alpaca.jpeg" />
    <animals label="animals" img-name="pig.jpeg" />
  </div>
</template>

<script>
import Animals from "./components/Animals";

export default {
  name: "App",
  components: {
    Animals,
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
