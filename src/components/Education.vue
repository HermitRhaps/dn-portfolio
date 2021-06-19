<template>
  <div id="education">
    <div class="container">
      <div class="body">
        <div class="content-img">
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
  max-width: 70%;
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
  max-width: 65%;
}
.current {
  opacity: 1;
}
@media only screen and (min-device-width: 320px) and (max-device-width: 1023px) {
  .content-img {
    width: 100vw;
    flex-direction: column;
    justify-content: center;
  }
  .content-img .img:nth-child(1) {
    align-self: flex-start;
    max-width: 75%;
  }
  .content-img .img span {
    font-size: 6vw;
  }
  .content-img .img:nth-child(2) {
    align-self: center;
    max-width: 100%;
    display: flex;
    align-items: flex-end;
  }
  .content-img .img span:last-of-type {
    font-size: 5vw;
  }
}
</style>