<template>
  <div id="app">
    <div class="container">
      <Initial />
      <About />
    </div>
  </div>
</template>

<script>
import Initial from "./components/Initial.vue";
import About from "./components/About.vue";
export default {
  name: "App",
  components: {
    Initial,
    About,
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
}
#app {
  height: 100vh;
  width: 100vw;
  background-color: rgb(236, 238, 233);
}
</style>
