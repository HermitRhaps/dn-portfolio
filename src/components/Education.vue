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
  width: 100%;
  padding: 10rem 1rem;
  display: flex;
  align-items: center;
  justify-content: center;
}
.current {
  opacity: 0;
}
.content-img {
  max-width: 70%;
  padding: 1rem;
  display: flex;
}
.content-img .img {
  max-width: 85%;
  height: auto;
  padding: 1rem;
  display: flex;
  flex-direction: column;
}

.content-img .img span {
  font-size: 3rem;
}
.content-img .img img {
  max-width: 75%;
  height: auto;
}

.body::before {
  content: "Education";
  right: 1rem;
  top: 1rem;
  display: block;
  position: absolute;
  font-size: 5rem;
  padding: 1rem;
  border-right: 1rem solid black;
}
.content-img .img span:last-of-type {
  font-size: 2rem;
}
.current {
  opacity: 1;
}
.invert .content-img img {
  filter: invert(1);
}
@media only screen and (min-device-width: 320px) and (max-device-width: 1023px) {
  .body::before {
    border-right: 0.25rem solid black;
  }
  .content-img {
    min-width: 75%;
    flex-direction: column;
    justify-content: center;
  }
  .body::before {
    font-size: 7vh;
  }
  .img:nth-child(2) {
    align-self: flex-end;
    text-align: end;
  }
  .content-img .img span {
    font-size: 2rem;
  }
  .content-img .img span:last-of-type {
    font-size: 1rem;
  }
  .content-img .img img {
    display: none;
  }
  .content-img .img span:nth-last-child(1) {
    content: "";
    display: flex;
    height: 0.05rem;
    width: 100%;
    background-color: black;
  }
}
</style>