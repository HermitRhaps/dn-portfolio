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
        <a href="#">
          <div class="up">
            <img src="../assets/arrow-down.svg" alt="arrow" />
          </div>
        </a>
        <a href="#education">
          <div class="down">
            <img src="../assets/arrow-down.svg" alt="arrow" />
          </div>
        </a>
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
.header {
  background-image: url("../assets/about.jpeg");
}
.body {
  padding: 0 5vw;
}
.skills {
  width: 40vw;
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
</style>