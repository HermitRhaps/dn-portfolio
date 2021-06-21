<template>
  <div id="education">
    <div class="container">
      <div class="body">
        <div class="content-img">
          <div class="img">
            <span>BNTU</span>
            <img src="../assets/bntu.jpeg" alt="content-img-1" />
            <span>Software engineer</span>
          </div>
          <div class="img">
            <span>TeachMeSkills</span>
            <img src="../assets/courses.jpeg" alt="content-img-2" />
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
  padding: 10vh 4vw;
  display: flex;
  overflow: hidden;
  align-items: center;
  justify-content: center;
}
.current {
  opacity: 0;
}
.content-img {
  max-width: 100%;
  height: 100%;
  padding: 1vh;
  display: flex;
}
.content-img .img {
  max-width: 35%;
  height: auto;
  display: flex;
  flex-direction: column;
  padding: 1vh;
}

.content-img .img span {
  font-size: 3vw;
}
.content-img .img img {
  max-width: 60vw;
  height: auto;
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
.current {
  opacity: 1;
}
.invert .content-img img {
  filter: invert(1);
}
@media only screen and (min-device-width: 320px) and (max-device-width: 1023px) {
  .content-img {
    min-width: 75vw;
    flex-direction: column;
    justify-content: center;
  }
  .body::before {
    font-size: 7vh;
  }
  .content-img .img {
    max-width: 65%;
    padding: 5vw;
  }
  .img:nth-child(2) {
    align-self: flex-end;
    text-align: end;
  }
  .content-img .img span {
    font-size: 6vw;
  }
  .content-img .img span:last-of-type {
    font-size: 4vw;
  }
  .content-img .img img {
    display: none;
  }
  .content-img .img span:nth-last-child(1) {
    content: "";
    display: flex;
    height: 0.05vh;
    width: 100%;
    background-color: black;
  }
}
</style>