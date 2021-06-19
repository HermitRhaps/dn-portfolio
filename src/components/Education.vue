<template>
  <div id="education">
    <div class="container education">
      <div class="body">
        <div class="content-img">
          <div class="img">
            <span>School</span>
            <img src="../assets/school.jpeg" alt="content-img-1" />
            <span>11 years</span>
          </div>
          <div class="img">
            <span>BNTU</span>
            <img src="../assets/books-img.jpeg" alt="content-img-2" />
            <span>Software engineer</span>
          </div>
          <div class="img">
            <span>TeachMeSkills</span>
            <img src="../assets/courses.jpeg" alt="content-img-3" />
            <span>Student Lab</span>
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
.body {
  height: 100vh;
  width: 100vw;
  padding: 5vw;
  display: flex;
  align-items: center;
  justify-content: center;
}
.current {
  opacity: 0;
}
.content-img {
  width: 85vw;
  height: 100%;
  padding: 1vh;
  display: flex;
}
.content-img .img {
  width: 100%;
  max-height: 75%;
  display: flex;
  flex-direction: column;
  padding: 1vh;
}

.content-img .img span {
  font-size: 3vw;
}
.content-img .img img {
  height: auto;
  min-width: 10%;
}

.body::before {
  content: "Education";
  right: 1vw;
  top: 1vw;
  display: block;
  position: absolute;
  font-size: 10vh;
  padding: 1vw;
  border-right: 1vw solid black;
}
.content-img .img span:last-of-type {
  font-size: 2vw;
}
.content-img .img:nth-child(1) {
  align-self: flex-start;
  max-width: 30%;
}
.content-img .img:nth-child(2) {
  align-self: center;
  max-width: 25%;
}
.content-img .img:nth-child(3) {
  align-self: flex-end;
  max-width: 45%;
}

@media only screen and (min-device-width: 320px) and (max-device-width: 1023px) {
}
</style>