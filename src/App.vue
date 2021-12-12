<template>
  <div id="app">
    <h1 class="title">Welcome to our Farm!</h1>
    <Animals class="card" label="animals" img-name="alpaca.jpeg" />
    <Animals class="card" label="animals" img-name="pig.jpeg" />
    <Animals class="card" label="animals" img-name="buffalo.jpeg" />
    <Animals class="card" label="animals" img-name="elephant.jpeg" />
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
body {
  margin: 0;
  color: rgb(70, 63, 58);
  font-family: arial;
  background: rgb(42, 146, 73);
}

p {
  font-size: 5rem;
}
</style>
