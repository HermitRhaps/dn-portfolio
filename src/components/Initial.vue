<template>
  <div id="initial">
    <div class="container">
      <div class="header">
        <div class="logo-holder">
          <img src="../assets/logo.svg" alt="logo" class="logo" />
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
          <div class="part" data-part="3" />
          <div class="part" data-part="4" />
        </div>
      </div>
      <div class="footer">
        <a href="#about">
          <div class="down-holder">
            <img src="../assets/arrow-down.svg" alt="down" />
          </div>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Initial",
  mounted: function () {
    document.addEventListener("mouseover", function (e) {
      if (e.target.classList.contains("part")) {
        document.querySelectorAll(".part").forEach((el) => {
          if (el.dataset.part !== e.target.dataset.part) {
            el.style["opacity"] = "0";
          } else {
            el.classList.add("part-active");
          }
        });
      }
    });
    document.addEventListener("mouseover", function (e) {
      if (!e.target.classList.contains("part")) {
        document.querySelectorAll(".part").forEach((el) => {
          el.classList.remove("part-active");
          el.style["opacity"] = "1";
        });
      }
    });
  },
  data: function () {
    return {};
  },
  methods: {},
};
</script>

<style scoped>
.header {
  display: flex;
  justify-content: center;
  flex-direction: column;
  text-align: center;
  position: relative;
}
.logo-holder {
  padding: 0.45vw;
}
.logo {
  min-width: 6vw;
  max-width: 8vw;
  filter: invert(1);
}
.author-holder {
  padding: 0.15vw;
  font-size: 3vw;
}
.author-holder > span {
  position: relative;
  padding: 1vw;
  display: inline-block;
}
.author-holder > span::after {
  content: "Frontend Developer";
  position: absolute;
  font-size: 1.2vw;
  right: 0;
  bottom: 0;
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
  font-size: 1.2vw;
  font-size: 2vw;
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
  font-size: 1.2vw;
  font-size: 2vw;
  bottom: -5vh;
}
.part:nth-child(3)::before {
  content: "Knowledge.";
  position: absolute;
  font-size: 1.2vw;
  font-size: 2vw;
  bottom: -5vh;
}
.part:nth-child(4)::before {
  content: "Talk w/ me.";
  position: absolute;
  font-size: 1.2vw;
  font-size: 2vw;
  bottom: -5vh;
}
.part:nth-child(3) {
  background-image: url("../assets/skills.jpeg");
  background-position: center;
  background-repeat: no-repeat;
  transition-duration: 2s;
}
.part:nth-child(4) {
  background-image: url("../assets/talk.jpeg");
  background-position: center;
  background-repeat: no-repeat;
  transition-duration: 2s;
}
.part:nth-child(1):hover:before {
  font-size: 5vw;
  top: -11.5vh;
  text-decoration: underline;
}
.part:nth-child(2):hover:before {
  font-size: 5vw;
  top: -11.5vh;
  text-decoration: underline;
}
.part:nth-child(3):hover:before {
  font-size: 5vw;
  top: -11.5vh;
  text-decoration: underline;
}
.part:nth-child(4):hover:before {
  font-size: 5vw;
  top: -11.5vh;
  text-decoration: underline;
}
.part:nth-child(1):hover {
  background-position: bottom;
  background-size: cover;
}
.part:nth-child(2):hover {
  background-position: bottom;
  background-size: cover;
}
.part:nth-child(3):hover {
  background-position: bottom;
  background-size: cover;
}
.part-active {
  position: absolute;
  height: 100%;
  width: 100%;
  transition-duration: 3s;

  z-index: 2;
}
.part:nth-child(4):hover {
  background-position: bottom;
  background-size: cover;
  backdrop-filter: inherit;
}

.down-holder {
  display: flex;
  justify-content: flex-end;
  align-items: center;
  text-align: center;
  padding: 1vh;
  position: absolute;
  bottom: 0;
  right: 0;
}
.down-holder > img {
  width: 5vw;
}
</style>