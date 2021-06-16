<template>
  <div id="about">
    <div class="container">
      <div class="header">
        <div class="icon">
          <img src="../assets/card-icon.svg" alt="icon" />
        </div>
        <div class="detail">
          <span>About me.</span>
        </div>
        <div class="up">
          <img src="../assets/arrow-down.svg" alt="arrow" />
        </div>
        <div class="down">
          <img src="../assets/arrow-down.svg" alt="arrow" />
        </div>
      </div>
      <div class="body">
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
        <div class="skills">
          <div class="s-item">
            <div class="i-icon">
              <img src="../assets/css.svg" alt="css" />
            </div>
            <div class="i-title">CSS</div>
          </div>
          <div class="s-item">
            <div class="i-icon">
              <img src="../assets/html.svg" alt="html" />
            </div>
            <div class="i-title">HTML</div>
          </div>
          <div class="s-item">
            <div class="i-icon">
              <img src="../assets/js.svg" alt="js" />
            </div>
            <div class="i-title">JS</div>
          </div>
          <div class="s-item">
            <div class="i-icon">
              <img src="../assets/database.svg" alt="db" />
            </div>
            <div class="i-title">SQL</div>
          </div>
          <div class="s-item">
            <div class="i-icon">
              <img src="../assets/github.svg" alt="github" />
            </div>
            <div class="i-title">Github</div>
          </div>
          <div class="s-item">
            <div class="i-icon">
              <img src="../assets/reactjs.svg" alt="react" />
            </div>
            <div class="i-title">React</div>
          </div>
          <div class="s-item">
            <div class="i-icon">
              <img src="../assets/nodejs.svg" alt="nodejs" />
            </div>
            <div class="i-title">Node JS</div>
          </div>
          <div class="s-item">
            <div class="i-icon">
              <img src="../assets/ui.svg" alt="ui/ux" />
            </div>
            <div class="i-title">UX/UI</div>
          </div>
          <div class="s-item">
            <div class="i-icon">
              <img src="../assets/database-orm.svg" alt="ORM" />
            </div>
            <div class="i-title">ORM</div>
          </div>
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
#about {
  height: 100vh;
  width: 100vw;
  background-color: rgb(236, 238, 233);
}
.container {
  height: 100%;
  width: 100%;
  position: relative;
}
.header {
  height: 25vh;
  overflow: hidden;
  background-image: url("../assets/about.jpeg");
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
}
.icon {
  background-color: black;
  border: 0.75vh solid rgb(236, 238, 233);
  padding: 1vh;
  z-index: 2;
  position: absolute;
  top: 20vh;
  left: 5vh;
}
.detail {
  padding: 1vh;
  z-index: 2;
  position: absolute;
  top: 24.9vh;
  left: 19vh;
  color: black;
  font-size: 6vh;
  text-decoration: underline;
}
.icon > img {
  filter: invert(1);
  width: 10vh;
}
.body {
  height: 75vh;
  padding: 10vh 5vh;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.description {
  font-size: 3vh;
  text-align: justify;
  width: 45vw;
}
.skills {
  width: 45vw;
  display: flex;
  flex-wrap: wrap;
  align-content: flex-start;
}
.s-item {
  height: 15vh;
  min-width: 8vw;
  background: black;
  color: white;
  display: flex;
  text-align: center;
  justify-content: center;
  flex-direction: column;
  font-size: 3vh;
  margin: 0.85vh;
}
.s-item > .i-icon > img {
  min-width: 4vw;
}
.up {
  padding: 1vh;
  z-index: 2;
  position: absolute;
  top: 25vh;
  right: 0vh;
  font-size: 6vh;
  text-decoration: underline;
}
.down {
  padding: 1vh;
  z-index: 2;
  position: absolute;
  bottom: 1vh;
  right: 0vh;
  font-size: 6vh;
  text-decoration: underline;
}
.up > img {
  transform: rotate(180deg);
  width: 5vw;
}

.down > img {
  width: 5vw;
}
</style>