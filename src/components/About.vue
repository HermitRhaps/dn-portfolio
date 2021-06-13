<template>
  <div class="container">
    <div class="blur" />
    <div class="author">
      <span class="author-detail">Dmitry Nemov</span>
    </div>
    <div class="content">
      <div class="main-content">
        <div class="content-title">
          <span class="content-detail">Frontend developer</span>
        </div>
        <div class="content-body">
          <div class="content-text">
            <p class="content-p">
              Cheers, i am frontend developer that have experience in commercial
              development using React / Redux / Saga and writing an API for
              interacting with relational databases using NodeJS / Express /
              ORM. Also familiar with the concept of pixel perfect site layout,
              testing and component styling using Bootstrap and Material-UI. In
              my free time, I deepen my knowledge of NodeJS with JWT / CRUD and
              basic knowledge of UX / UI design. I set a goal for myself in the
              future to achieve the position of team lead in the shortest
              possible time and to develop my own startup in the field of IT.
            </p>
          </div>
          <div class="content-links">
            <ul class="content-links-list">
              <li class="content-links-item">
                <a href="https://github.com/HermitRhaps" class="link"
                  ><img
                    src="../assets/github-fill.svg"
                    lt="github"
                    class="link-ico"
                /></a>
              </li>
              <li class="content-links-item">
                <a href="https://www.linkedin.com/in/dmitry-nemov-8659a41a6/">
                  <img
                    src="../assets/linkedin-box-fill.svg"
                    alt="linkedin "
                    class="link-ico"
                /></a>
              </li>
            </ul>
          </div>
          <div class="scroll-down">
            <img
              src="../assets/arrow-drop-down-line.svg"
              alt="linkedin"
              class="down"
            />
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
.container {
  height: 100vh;
  background: url("../assets/about-background.jpeg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  overflow: hidden;
  display: flex;
}
.blur {
  background: rgba(255, 255, 255, 0);
  backdrop-filter: blur(7px);
  width: 100%;
  height: 100vh;
  position: absolute;
}
.author {
  color: white;
  padding: 1rem;
  position: absolute;
  transform: rotate(-90deg);
  top: 5.9em;
  right: -12.6rem;
  font-size: 2rem;
  display: flex;
  align-items: center;
  z-index: 2;
}
.author::before {
  content: "";
  display: flex;
  width: 10rem;
  height: 0.3rem;
  margin: 0 1rem;
  background: white;
}
.content-detail {
  position: relative;
  z-index: 2;
}
.main-content {
  padding: 1.45rem 0.15rem;
  position: relative;
  color: white;
  width: 100vw;
}

.content-title {
  padding: 2rem 5rem;
  font-size: 5.5rem;
  margin: 1rem 0;
}
.content-title::before {
  content: "";
  top: 2rem;
  left: 1.65rem;
  border: 0.65rem solid white;
  position: absolute;
  padding: 5rem 15rem;
  background: rgba(19, 19, 19, 0.6);
}

.content-body {
  padding: 0 5rem;
  display: flex;
  flex-direction: column;
  text-align: justify;
}
.content-text {
  font-size: 1.75rem;
  max-width: 60%;
  background: rgba(13, 9, 70, 0.6);
  display: flex;
  padding: 3rem;
  margin: auto;
}

.content-text::before {
  content: "About me";
  color: white;
  transform: rotate(-90deg);
  display: block;
  left: 2rem;
  top: 1rem;
  position: relative;
  width: 100rem;
  height: 0.25rem;
  background: white;
  z-index: 1;
}

.content-text::after {
  content: "";
  top: 5rem;
  left: -36rem;
  transform: rotate(145deg);
  position: absolute;
  padding: 25rem 80rem;
  background: rgba(209, 153, 31, 1);
  z-index: 0;
}

.content-p {
  position: relative;
  z-index: 2;
}
.content-links {
  padding: 2rem 0;
  display: flex;
  z-index: 2;
  width: 100%;
  justify-content: center;
  margin: auto;
}
.content-links-list {
  display: flex;
  justify-content: center;
  align-items: center;
}
.content-links-item {
  width: 25%;
  margin: 0 1rem;
}

.link-ico {
  width: 4rem;
}
.link-ico:hover {
  transform: scale(1.2);
}
.scroll-down {
  display: flex;
  justify-content: center;
  padding: 1rem 0;
}
.down {
  min-width: 6rem;
  max-width: 8rem;
}
</style>