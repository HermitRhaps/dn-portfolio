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
                  <img src="../assets/nodejs.svg" alt="css" class="img" />
                </div>
                <div class="s-d-title"><span>NodeJS</span></div>
              </div>
              <div class="s-d">
                <div class="s-d-img">
                  <img src="../assets/database-orm.svg" alt="css" class="img" />
                </div>
                <div class="s-d-title"><span>ORM</span></div>
              </div>
              <div class="s-d">
                <div class="s-d-img">
                  <img src="../assets/ui.svg" alt="css" class="img" />
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
  justify-content: flex-end;
  position: relative;
  align-items: flex-end;
}
.s-item {
  background-color: rgb(30, 30, 36);
  padding: 2rem 0.25rem;
  margin: 1rem;
  height: 15vh;
  width: 65%;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
}
.s-item::before {
  background-color: rgb(30, 30, 36);
  content: "";
  position: absolute;
  width: 1rem;
  height: 100rem;
  right: -1rem;
}
.s-d-wrapper {
  width: 80%;
  display: flex;
  justify-content: space-around;
  z-index: 1;
  position: relative;
  align-items: center;
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
.s-d {
  display: flex;
  justify-content: center;
  align-content: center;
  flex-direction: column;
  text-align: center;
}
.img {
  min-width: 3rem;
  max-width: 5rem;
}
.logo {
  width: 10rem;
}
.s-d-title {
  font-size: 2rem;
}
.p-text {
  font-size: 3rem;
}
.content {
  width: 50vw;
  background-color: rgb(30, 30, 36);
  position: relative;
}

.part {
  left: -20rem;
  top: 1rem;
}

@media only screen and (min-device-width: 320px) and (max-device-width: 1023px) {
  .content::before {
    left: 6.1rem;
  }
  .s-list {
    background: rgb(30, 30, 36);
  }
  .s-item::before {
    width: 2rem;
    right: -1.2rem;
  }
  .img {
    min-width: 1rem;
    max-width: 1.3rem;
  }
  .header {
    height: 100vh;
  }
  .s-item {
    height: 100vh;
    margin: 0;
  }
  .s-d-wrapper {
    flex-direction: column;
  }
  .s-item {
    height: 100vh;
    width: 100%;
  }
  .s-d-title {
    font-size: 1.2rem;
  }
  .s-d {
    height: 7vh;
  }
}
</style>