<template>
  <div id="about">
    <div class="container">
      <div class="header">
        <div class="author">
          <span>Dmitry Nemov</span>
        </div>
        <div class="logo">
          <img src="../assets/dnLOGO.svg" alt="myLogo" />
        </div>

        <div class="job">
          <span>Frontend Developer</span>
        </div>
      </div>
      <div class="content">
        <div class="part">
          <span>A</span>
        </div>
        <div class="navigation">
          <ul>
            <li><a href="#about">About</a></li>
            <li><a href="#education">Education</a></li>
            <li><a href="#skills">Skills</a></li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "About",
};
</script>

<style scoped>
.header {
  width: 25vw;
  background-color: rgb(236, 238, 233);
  position: relative;
}
.content {
  width: 75vw;
  background-color: rgb(30, 30, 36);
  position: relative;
}
.author {
  position: absolute;
  mix-blend-mode: difference;
  color: white;
  font-size: 18rem;
  bottom: 2rem;
  z-index: 1;
  text-indent: 16.8rem;
  line-height: 11.4rem;
}
.logo {
  filter: invert(1);
  animation: logo 2s forwards;
}
.job {
  position: absolute;
  mix-blend-mode: difference;
  font-size: 5rem;
  color: white;
  top: bottom;
  right: -50rem;
  line-height: 5rem;
  z-index: 1;
  padding: 10.2rem;
}
.navigation {
  position: fixed;
  right: 0;
  text-align: right;
  padding: 5rem;
  font-size: 7rem;
  z-index: 1;
  color: rgb(236, 238, 233);
  mix-blend-mode: difference;
}
.navigation > ul > li > a {
  color: rgb(236, 238, 233);
  mix-blend-mode: difference;
}
.navigation > ul > li:hover {
  color: white;
  animation: navigation 0.3s forwards;
}

@keyframes logo {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

@keyframes navigation {
  from {
    filter: invert(0);
  }
  to {
    filter: invert(1);
  }
}

@media only screen and (min-device-width: 320px) and (max-device-width: 1023px) {
  .header {
    width: 40vw;
  }
  .author {
    padding: 1rem;
    font-size: 4.5rem;
    bottom: 1rem;
    text-indent: 4rem;
    line-height: 3rem;
  }
  .navigation {
    position: fixed;
    right: 0;
    text-align: right;
    padding: 3rem 1rem;
    font-size: 2rem;
    z-index: 1;
    color: rgb(236, 238, 233);
    mix-blend-mode: difference;
  }
  .job {
    position: absolute;
    mix-blend-mode: difference;
    font-size: 2rem;
    color: white;
    bottom: 9rem;
    left: 2rem;
    line-height: 2rem;
    z-index: 1;
    padding: 0;
  }
}
</style>