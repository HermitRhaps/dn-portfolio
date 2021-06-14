<template>
  <div id="education">
    <div class="container">
      <div class="header">
        <div class="e-time">
          <div class="e-part">
            <div class="e-year">2015-2020</div>
          </div>
          <div class="e-part">
            <div class="e-year">2020-2021</div>
          </div>
        </div>
      </div>
      <div class="content">
        <div class="part">
          <span>E</span>
        </div>
        <div class="e-description">
          <div class="e-d-item">
            BNTU
            <div class="e-d-after">Information technology software</div>
            <div class="e-d-before">Software Engineer</div>
          </div>
          <div class="e-d-item">
            TEACHMESKILLS
            <div class="e-d-after">Frontend Developer</div>
            <div class="e-d-before">Student with certificate</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Education",
};
</script>

<style scoped>
.header {
  width: 25vw;
  color: rgb(236, 238, 233);
  position: relative;
}
.content {
  width: 75vw;
  background-color: rgb(30, 30, 36);
  position: relative;
}
.e-time {
  display: flex;
  flex-direction: column;
  height: 100%;
  width: 35%;
  justify-content: space-around;
  position: absolute;
  padding: 20rem 0;
  top: 0;
  bottom: 0;
  left: 25rem;
  right: 0;
}
.e-description {
  display: flex;
  padding: 20rem 3rem;
  flex-direction: column;
  height: 100%;
  width: 35%;
  justify-content: space-around;
}
.e-part {
  height: 1.5%;
  background: rgb(30, 30, 36);
  position: relative;
}
.e-year {
  position: absolute;
  top: 1rem;
  right: 1rem;
  font-size: 2rem;
  color: black;
  width: 10vw;
}
.e-d-item {
  font-size: 5rem;
  color: rgb(236, 238, 233);
}
.e-d-before {
  font-size: 1.2rem;
}
.e-d-after {
  font-size: 1.75rem;
}

@media only screen and (min-device-width: 320px) and (max-device-width: 1023px) {
  .header {
    width: 40vw;
  }
  .e-time {
    padding: 5rem 0;
    left: 1rem;
    width: 95%;
  }
  .e-year {
    font-size: 1.5rem;
    right: 3rem;
  }
  .e-description {
    padding: 5rem 1rem;
  }
  .e-d-item {
    font-size: 2rem;
  }
  .e-d-before {
    font-size: 0.75rem;
  }
  .e-d-after {
    font-size: 1.25rem;
  }
}
</style>