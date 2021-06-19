<template>
  <div id="app">
    <div class="container">
      <Initial />
      <About />
      <Education />
      <Other />
    </div>
  </div>
</template>

<script>
import Initial from "./components/Initial.vue";
import About from "./components/About.vue";
import Education from "./components/Education.vue";
import Other from "./components/Other.vue";
export default {
  name: "App",
  components: {
    Initial,
    About,
    Education,
    Other,
  },
  mounted: function () {
    window.addEventListener("scroll", function () {
      document
        .elementFromPoint(window.scrollX, window.scrollY)
        .classList.add("current");
    });
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
#app,
#about,
#initial,
#education,
#other {
  height: 100vh;
  width: 100vw;
  background-color: rgb(236, 238, 233);
}
.container {
  height: 100vh;
  width: 100%;
  /* overflow: hidden; */
}
.header {
  height: 25vh;
  overflow: hidden;
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  position: relative;
}
.body {
  min-height: 75vh;
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: relative;
}
.description {
  font-size: 3vh;
  text-align: justify;
  width: 45vw;
}
.icon {
  background-color: black;
  border: 0.35vh solid rgb(236, 238, 233);
  padding: 1vh;
  position: absolute;
  top: 1vh;
  left: 1vh;
}
.detail {
  padding: 1vh;
  z-index: 2;
  position: absolute;
  bottom: -2.5vh;
  left: 15vh;
  color: white;
  font-size: 7vw;
  text-shadow: 1px 0 0 black, 0 1px 0 black, -1px 0 0 black, 0 -1px 0 black;
}
.icon > img {
  filter: invert(1);
  width: 8vh;
}
.up {
  padding: 1vh;
  z-index: 2;
  position: fixed;
  bottom: 0vh;
  right: 0vh;
  font-size: 6vh;
  text-decoration: underline;
}
.up > img {
  transform: rotate(180deg);
  width: 5vw;
  opacity: 0;
}

.up > img:hover {
  border-radius: 50%;
  background: white;
  filter: invert(1);
}
@media only screen and (min-device-width: 320px) and (max-device-width: 1023px) {
  .icon {
    background-color: black;
    border: 1vh solid rgb(236, 238, 233);
    padding: 1vh;
    z-index: 2;
    position: absolute;
    top: 1vh;
    left: 1vh;
    border-radius: 50%;
  }
  .detail {
    top: 2vh;
    left: 15vh;
    font-size: 13vw;
  }
  .body {
    flex-direction: column;
  }
  .description {
    padding: 2vh 0;
    font-size: 2.2vh;
    width: 87vw;
  }

  .up {
    right: -1vh;
  }
  .up > img {
    width: 6vw;
  }
  .body {
    height: 85vh;
  }
}
</style>
