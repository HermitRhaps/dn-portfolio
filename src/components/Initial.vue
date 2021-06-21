<template>
  <div id="initial">
    <div class="container">
      <div class="header">
        <div class="logo-holder">
          <img src="../assets/logo.svg" alt="logo" class="logo" />
        </div>
        <div class="theme">
          <img src="../assets/theme.svg" alt="theme" />
        </div>
        <div class="author-holder">
          <span>Dmitry Nemov</span>
        </div>
      </div>
      <div class="i-body">
        <div class="parts">
          <a href="#about" class="part" data-part="1"><div data-part="1" /></a>
          <a href="#education" class="part" data-part="2"
            ><div data-part="2"
          /></a>
          <a href="#other" class="part" data-part="3"><div data-part="3" /></a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Initial",
  mounted: function () {
    document.querySelector(".theme").addEventListener("click", function () {
      document.querySelector(".container").classList.toggle("invert");
    });
  },
  data: function () {
    return {};
  },
  methods: {},
};
</script>
<style>
.invert {
  filter: invert(1);
}
.invert .i-body > .parts > .part {
  filter: invert(1);
  color: white;
}
.invert .header {
  filter: invert(1);
  z-index: 2;
  color: white;
}
.invert .logo-holder {
  filter: invert(1);
  z-index: 2;
}
.invert .theme {
  filter: invert(1);
  z-index: 2;
}
</style>
<style scoped>
.header {
  display: flex;
  justify-content: center;
  flex-direction: column;
  text-align: center;
  position: relative;
}
.logo-holder {
  width: 100%;
  padding: 0.45rem;
}
.logo {
  max-width: 5%;
  height: auto;
  filter: invert(1);
}
.author-holder {
  padding: 0.15vw;
  font-size: 4rem;
  height: auto;
}
.author-holder > span {
  position: relative;
  padding: 1rem;
}
.author-holder > span::after {
  content: "Frontend Developer";
  position: absolute;
  font-size: 2rem;
  right: 0;
  top: -0.45rem;
  transition-duration: 2s;
}
.parts {
  display: flex;
  padding: 5vh;
  justify-content: center;
}
.part {
  min-width: 13vw;
  min-height: 50vh;
  padding: 0.15vh;
  position: relative;
  color: rgb(30, 30, 36);
}
.part:nth-child(1) {
  background-image: url("../assets/about.jpeg");
  background-position: center;
  background-repeat: no-repeat;
  transition-duration: 2s;
}
.part:nth-child(1)::before {
  content: "About.";
  position: absolute;
  font-size: 2rem;
  bottom: -5vh;
}
.part:nth-child(2) {
  background-image: url("../assets/education.jpeg");
  background-position: center;
  background-repeat: no-repeat;
  transition-duration: 2s;
}
.part:nth-child(2)::before {
  content: "Education.";
  position: absolute;
  font-size: 2rem;
  bottom: -5vh;
}
.part:nth-child(3)::before {
  content: "Other info.";
  position: absolute;
  font-size: 2rem;
  bottom: -5vh;
}
.part:nth-child(3) {
  background-image: url("../assets/skills.jpeg");
  background-position: center;
  background-repeat: no-repeat;
  transition-duration: 2s;
}

.part:nth-child(1):hover:before,
.part:nth-child(2):hover:before,
.part:nth-child(3):hover:before {
  font-size: 3vw;
  top: 25vh;
  text-align: center;
  width: 100vw;
  color: rgb(236, 238, 233);
  animation: textShownUp 1.5s forwards;
  text-shadow: 1px 0 0 black, 0 1px 0 black, -1px 0 0 black, 0 -1px 0 black;
}

.part:nth-child(1):hover,
.part:nth-child(2):hover,
.part:nth-child(3):hover {
  background-size: cover;
  min-width: 75%;
  overflow: hidden;
}

.theme {
  position: absolute;
  top: 0;
  padding: 1rem;
}
.theme > img {
  min-width: 5rem;
  height: auto;
}
@keyframes textShownUp {
  0% {
    opacity: 0;
    filter: blur(10px);
  }
  100% {
    opacity: 1;
    filter: blur(0px);
  }
}
@media only screen and (min-device-width: 320px) and (max-device-width: 1023px) {
  .theme img {
    min-width: 3rem;
  }
  .logo {
    max-width: 20%;
    height: auto;
  }
  .author-holder > span {
    padding: 1rem;
    font-size: 2rem;
  }
  .author-holder > span::after {
    font-size: 1rem;
  }
  .parts {
    min-width: 90vw;
  }
  .part {
    min-width: 24.5vw;
    min-height: 60vh;
  }
  .part:nth-child(1)::before,
  .part:nth-child(2)::before,
  .part:nth-child(3)::before {
    bottom: -4vh;
    font-size: 3vw;
  }
  .part:nth-child(1):hover:before,
  .part:nth-child(2):hover:before,
  .part:nth-child(3):hover:before {
    display: none;
  }

  .part:nth-child(1):hover,
  .part:nth-child(2):hover,
  .part:nth-child(3):hover {
    display: none;
  }
}
</style>