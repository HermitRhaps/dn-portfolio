<template>
  <div id="about">
    <div class="container about">
      <div class="body">
        <div class="header">
          <span
            >A young specialist with an irrepressible desire to develop.</span
          >
        </div>
        <div class="content-img">
          <img src="../assets/old_comp.jpeg" alt="content-img" />
        </div>
        <div class="description">
          <span>
            and i have experience in commercial development using
            React/Redux/Saga for frontend part and writing an API for
            interacting with relational databases using Node JS/Express/ORM.
            Also familiar with the concept of pixel perfect site layout, testing
            and component styling using Bootstrap and Material-UI. In my free
            time, I deepen my knowledge of NodeJS and JWT/CRUD and study UX/UI
            design. I set a goal for myself in the future to achieve the
            position of team lead in the shortest possible time and to develop
            my own startup in the field of IT.</span
          >
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
.body {
  height: 100vh;
  width: 100vw;
  padding: 5rem;
  position: relative;
}
.content-img {
  max-width: 100vh;
  height: auto;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  border-left: 0.7rem solid black;
  transform: translateX(-100vw);
}
.header {
  position: absolute;
  top: 0;
  left: 1rem;
  font-size: 2.2rem;
  opacity: 0;
  transition-duration: 2s;
}
.description::before {
  content: "👋 i'm Nemov Dmitry";
  display: block;
  position: absolute;
  font-size: 3rem;
  top: -3rem;
  right: 0;
}
.content-img > img {
  width: 95%;
  height: auto;
}
.current > .header {
  opacity: 1;
}
.current > .header span::before {
  content: "";
  display: block;
  font-size: 5rem;
  width: 100%;
  height: 0.55rem;
  background: black;
  top: -6rem;
  left: -0.6rem;
}
.current > .description {
  opacity: 1;
}
.current > .description span::after {
  content: "";
  display: block;
  width: 100%;
  height: 0.55rem;
  background: black;
  margin: 1rem 0;
}
.invert > .description span::after {
  filter: invert(0);
  background: white;
}
.invert .description span::before {
  filter: invert(1);
  color: white;
}
.invert .header span::before {
  background: white;
}
.invert .content-img img {
  filter: invert(1);
}
.current > .content-img {
  animation: contentImgMoveIn 3s forwards;
}
.current > .description > span::before {
  animation: contentBeforeMoveIn 3s forwards;
}

.current > .content-img::before {
  content: "About";
  display: block;
  position: absolute;
  font-size: 5rem;
  top: -6rem;
  left: -0.6rem;
}
.description {
  font-size: 1vw;
  position: relative;
  display: flex;
  justify-content: space-around;
  flex-direction: column;
  padding: 1rem;
  opacity: 0;
  transition-duration: 4s;
  position: relative;
}

/* animations  */
@keyframes contentImgMoveIn {
  0% {
    transform: translateX(-100vw);
  }
  100% {
    transform: translateX(0vw);
  }
}
@keyframes contentBeforeMoveIn {
  0% {
    transform: translateX(100vw);
  }
  100% {
    transform: translateX(0vw);
  }
}
@media only screen and (min-device-width: 320px) and (max-device-width: 1023px) {
  .body {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
  }
  .header {
    padding: 1vh;
    font-size: 3vw;
  }
  .description {
    font-size: 3vw;
    height: 20%;
  }
  .content-img {
    padding: 1vh;
    font-size: 3vw;
  }
  .description::before {
    font-size: 1.5rem;
    top: -7rem;
    right: 2rem;
  }
}
@media only screen and (min-device-width: 1024px) and (max-device-width: 1366px) {
  .body {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
  }
  .header {
    padding: 0.1rem;
    font-size: 2rem;
  }
  .description {
    font-size: 1.5rem;
  }
  .content-img {
    width: 50%;
    padding: 0.51rem;
  }
  .current > .content-img::before {
    font-size: 2rem;
    top: -3rem;
  }
  .description::before {
    font-size: 2rem;
    top: -1.5rem;
    right: 2rem;
  }
}
</style>