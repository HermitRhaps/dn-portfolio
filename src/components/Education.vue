<template>
  <div id="education">
    <div class="container">
      <div class="header"></div>
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

.e-description {
  display: flex;
  padding: 0 5vw;
  flex-direction: column;
  height: 100vh;
  width: 40%;
  justify-content: center;
}
.e-part {
  min-height: 0.75rem;
  width: 100%;
  background: rgb(30, 30, 36);
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

  .e-description {
    padding: 5rem 1rem;
  }
  .e-d-item {
    font-size: 1.65rem;
  }
  .e-d-before {
    font-size: 0.75rem;
  }
  .e-d-after {
    font-size: 1.25rem;
  }
}
</style>