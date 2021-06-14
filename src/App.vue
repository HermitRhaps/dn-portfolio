<template>
  <div id="app">
    <About />
    <Education />
  </div>
</template>

<script>
import About from "./components/About";
import Education from "./components/Education";
export default {
  name: "App",
  components: {
    About,
    Education,
  },
};
</script>

<style >
* {
  user-select: none;
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  text-decoration: none;
  list-style: none;
  font-family: "Roboto Slab", serif;
}
html {
  scroll-behavior: smooth;
}
body {
  overflow: hidden;
  background-color: rgb(236, 238, 233);
}
.container {
  height: 100vh;
  display: flex;
  overflow: hidden;
}
.part {
  font-size: 5rem;
  color: white;
  position: absolute;
  top: 0;
  left: 2rem;
}
@media only screen and (min-device-width: 320px) and (max-device-width: 1023px) {
  .part {
    font-size: 3rem;
    left: 1rem;
  }
}
</style>
