<template>
  <div id="app">
    <div class="container">
      <Initial />
      <About />
      <Education />
    </div>
  </div>
</template>

<script>
import Initial from "./components/Initial.vue";
import About from "./components/About.vue";
import Education from "./components/Education.vue";
export default {
  name: "App",
  components: {
    Initial,
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
}
#app,
#about,
#initial,
#education {
  height: 100vh;
  width: 100vw;
  background-color: rgb(236, 238, 233);
}
.container {
  height: 100%;
  width: 100%;
  position: relative;
}
.header {
  height: 25vh;
  overflow: hidden;
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
}
.body {
  height: 75vh;
  padding: 10vh 5vh;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.description {
  font-size: 3vh;
  text-align: justify;
  width: 45vw;
}
.icon {
  background-color: black;
  border: 0.75vh solid rgb(236, 238, 233);
  padding: 1vh;
  z-index: 2;
  position: absolute;
  top: 20vh;
  left: 5vh;
}
.detail {
  padding: 1vh;
  z-index: 2;
  position: absolute;
  top: 24.9vh;
  left: 19vh;
  color: black;
  font-size: 6vh;
  text-decoration: underline;
}
.icon > img {
  filter: invert(1);
  width: 10vh;
}
.up {
  padding: 1vh;
  z-index: 2;
  position: absolute;
  top: 25vh;
  right: 0vh;
  font-size: 6vh;
  text-decoration: underline;
}
.down {
  padding: 1vh;
  z-index: 2;
  position: absolute;
  bottom: 1vh;
  right: 0vh;
  font-size: 6vh;
  text-decoration: underline;
}
.up > img {
  transform: rotate(180deg);
  width: 5vw;
}
.down > img {
  width: 5vw;
}
.down-holder > img:hover,
.up > img:hover,
.down > img:hover {
  padding: 1vh;
  border-radius: 50%;
  background: white;
  filter: invert(1);
}
</style>
