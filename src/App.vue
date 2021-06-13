<template>
  <div id="app">
    <About />
    <!-- <Projects /> -->
  </div>
</template>

<script>
import About from "./components/About";
// import Projects from "./components/Projects";
export default {
  name: "App",
  components: {
    About,
    // Projects,
  },
};
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  text-decoration: none;
  list-style: none;
}
body {
  background: black;
}
#app {
  font-family: "Roboto Slab", serif;
}
</style>
