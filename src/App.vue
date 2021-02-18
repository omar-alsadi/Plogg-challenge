<template>
  <div id="app">
    <h2>OMAR ALSADI</h2>
    <span>
      Create a VueJs Component that has two input fields and displays the sum of
      the values in them.</span
    >
    <Inputs />
  </div>
</template>

<script>
import Inputs from "./components/Inputs";

export default {
  name: "App",
  components: {
    Inputs,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 600px;
  margin: 3rem auto;
}

h2 {
  color: #42b983;
}
</style>
