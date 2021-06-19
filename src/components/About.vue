<template>
  <div id="about">
    <div class="container about">
      <div class="body">
        <div class="header">
          <span
            >Lorem Ipsum is simply dummy text of the printing and typesetting
            industry.</span
          >
        </div>
        <div class="content-img">
          <img src="../assets/old_comp.jpeg" alt="content-img" />
        </div>
        <div class="description">
          <span
            >Lorem Ipsum is simply dummy text of the printing and typesetting
            industry. Lorem Ipsum has been the industry's standard dummy text
            ever since the 1500s, when an unknown printer took a galley of type
            and scrambled it to make a type specimen book. It has survived not
            only five centuries, but also the leap into electronic typesetting,
            remaining essentially unchanged. It was popularised in the 1960s
            with the release of Letraset sheets containing Lorem Ipsum passages,
            and more recently with desktop publishing software like Aldus
            PageMaker including versions of Lorem Ipsum.</span
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
  padding: 5vw;
  position: relative;
}
.content-img {
  width: 40vw;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  border-left: 0.7vw solid black;
  transform: translateX(-100vw);
}
.header {
  position: absolute;
  top: 0;
  left: 1vw;
  font-size: 2.2vw;
  opacity: 0;
  transition-duration: 2s;
}
.description {
  opacity: 0;
  transition-duration: 4s;
  position: relative;
}
.description > span::before {
  content: "👋 i'm Nemov Dmitry";
  display: block;
  position: absolute;
  font-size: 3vw;
  top: 7vw;
  right: -0.6vw;
}
.content-img > img {
  width: 95%;
}
.current > .header {
  opacity: 1;
}
.current > .header span::before {
  content: "";
  display: block;
  font-size: 5vw;
  width: 100%;
  height: 1vh;
  background: black;
  top: -6vw;
  left: -0.6vw;
}

.current > .description {
  opacity: 1;
}
.current > .description span::after {
  content: "";
  display: block;
  width: 100%;
  height: 1vh;
  background: black;
  margin: 1vw 0;
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
  font-size: 5vw;
  top: -6vw;
  left: -0.6vw;
}
.description {
  font-size: 1.5vw;
  display: flex;
  justify-content: space-around;
  flex-direction: column;
  height: 100%;
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
}
</style>