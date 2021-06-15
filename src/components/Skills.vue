<template>
  <div id="skills">
    <div class="container">
      <div class="header">
        <div class="s-list">
          <div class="s-item">
            <div class="s-d-wrapper">
              <div class="s-d">
                <div class="s-d-img">
                  <img src="../assets/html.svg" alt="html" class="img" />
                </div>
                <div class="s-d-title"><span>HTML</span></div>
              </div>
              <div class="s-d">
                <div class="s-d-img">
                  <img src="../assets/css.svg" alt="css" class="img" />
                </div>
                <div class="s-d-title"><span>CSS</span></div>
              </div>
              <div class="s-d">
                <div class="s-d-img">
                  <img src="../assets/js.svg" alt="js" class="img" />
                </div>
                <div class="s-d-title"><span>JS</span></div>
              </div>
              <div class="s-d">
                <div class="s-d-img">
                  <img src="../assets/database.svg" alt="js" class="img" />
                </div>
                <div class="s-d-title"><span>SQL</span></div>
              </div>
              <div class="s-d">
                <div class="s-d-img">
                  <img src="../assets/github.svg" alt="js" class="img" />
                </div>
                <div class="s-d-title"><span>GitHub</span></div>
              </div>
            </div>
          </div>
          <div class="s-item">
            <div class="s-d-wrapper">
              <div class="s-d">
                <div class="s-d-img">
                  <img src="../assets/reactjs.svg" alt="html" class="img" />
                </div>
                <div class="s-d-title"><span>React</span></div>
              </div>

              <div class="s-d">
                <div class="s-d-img">
                  <img src="../assets/js.svg" alt="css" class="img" />
                </div>
                <div class="s-d-title"><span>NodeJS</span></div>
              </div>
              <div class="s-d">
                <div class="s-d-img">
                  <img src="../assets/js.svg" alt="css" class="img" />
                </div>
                <div class="s-d-title"><span>ORM</span></div>
              </div>
              <div class="s-d">
                <div class="s-d-img">
                  <img src="../assets/js.svg" alt="css" class="img" />
                </div>
                <div class="s-d-title"><span>UX / UI</span></div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="content">
        <div class="part">
          <span>S</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Skills",
};
</script>

<style scoped>
.header {
  width: 50vw;
  color: rgb(236, 238, 233);
  position: relative;
}
.s-list {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  position: relative;
  align-items: center;
}
.s-item {
  background-color: rgb(30, 30, 36);
  padding: 2rem;
  height: 15vh;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
}
.s-d-wrapper {
  width: 80%;
  display: flex;
  justify-content: space-around;
  padding: 0 4rem;
  z-index: 1;
  position: relative;
  align-items: center;
}

.s-d {
  display: flex;
  justify-content: center;
  align-content: center;
  flex-direction: column;
  text-align: center;
}
.img {
  width: 5rem;
}
.s-d-title {
  font-size: 2rem;
}

.content {
  width: 50vw;
  background-color: rgb(30, 30, 36);
  position: relative;
}
.content::before {
  position: absolute;
  display: block;
  content: "";
  width: 60rem;
  height: 60rem;
  transform: rotate(45deg);
  background-color: rgb(30, 30, 36);
  top: -30rem;
  left: -20.5rem;
}
.part {
  left: -20rem;
  top: 1rem;
}
</style>