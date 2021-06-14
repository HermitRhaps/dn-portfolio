<template>
  <div class="container-list">
    <div class="content">
      <div class="content-line" />
      <div class="content-card">
        <div class="card-detail">
          <div class="detail-title">
            <span>PokePocket.</span>
          </div>
          <div class="detail-body">
            <span>Fetching data from Pokémon data RESTful API.</span>
          </div>
          <div class="detail-links">
            <a href="https://github.com/HermitRhaps/PokePocket" class="link"
              ><img
                src="../assets/github-fill.svg"
                lt="github"
                class="link-ico"
            /></a>
          </div>
        </div>
        <div class="card-img-wrapper">
          <img src="../assets/poke.png" alt="pokePocket" class="card-img" />
        </div>
      </div>

      <div class="content-card">
        <div class="card-detail">
          <div class="detail-title">
            <span>Weather-app</span>
          </div>
          <div class="detail-body">
            <span
              >App that use OpenWeatherMap API tools to find current forecast,
              hourly forecast and daily forecast base on city that user
              select.</span
            >
          </div>
          <div class="detail-links">
            <a href="https://github.com/HermitRhaps/Weather-app" class="link"
              ><img
                src="../assets/github-fill.svg"
                lt="github"
                class="link-ico"
            /></a>
          </div>
        </div>
        <div class="card-img-wrapper">
          <img src="../assets/weather.png" alt="Weather-app" class="card-img" />
        </div>
      </div>

      <div class="content-card">
        <div class="card-detail">
          <div class="detail-title">
            <span>Todo-metr.</span>
          </div>
          <div class="detail-body">
            <span
              >Simple Frontend & Backend application to create/edit/delete todos
              with function to search them.</span
            >
          </div>
          <div class="detail-links">
            <a href="https://github.com/HermitRhaps/Todo-metr" class="link"
              ><img
                src="../assets/github-fill.svg"
                lt="github"
                class="link-ico"
            /></a>
          </div>
        </div>
        <div class="card-img-wrapper">
          <img src="../assets/no-image.jpg" alt="Todo-metr" class="card-img" />
        </div>
      </div>

      <div class="content-card">
        <div class="card-detail">
          <div class="detail-title">
            <span>Soon.</span>
          </div>
          <div class="detail-body">
            <span></span>
          </div>
          <div class="detail-links">
            <!-- <a href="https://github.com/HermitRhaps" class="link"
              ><img
                src="../assets/github-fill.svg"
                lt="github"
                class="link-ico"
            /></a> -->
          </div>
        </div>
        <div class="card-img-wrapper">
          <img src="../assets/soon.jpeg" alt="Soon" class="card-img" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Projects",
  data() {
    return {};
  },
};
</script>

<style scoped>
.container-list {
  min-height: 100vh;
  background: url("../assets/about-background.jpeg");
  background-position: bottom;
  background-repeat: no-repeat;
  background-size: cover;
  overflow: hidden;
}
.content {
  width: 100%;
  display: flex;
  justify-content: space-around;

  flex-wrap: wrap;
  position: relative;
}

.content::after {
  content: "";
  top: -61.85rem;
  left: -36rem;
  transform: rotate(145deg);
  position: absolute;
  padding: 35rem 35rem;
  background: #d14646;
}
.content-line::after {
  content: "";
  top: 0rem;
  right: -123.9rem;
  transform: rotate(20deg);
  position: absolute;
  width: 150rem;
  height: 170rem;
  background: #d14646;
  z-index: 0;
}
.content-line {
  position: absolute;
  top: 0;
  width: 100vw;
  height: 50vh;
  padding: 1rem;
  background: rgb(29, 39, 177);
}
.content-card {
  background: white;
  padding: 0.15rem;
  width: 25%;
  display: flex;
  justify-content: center;
  align-content: center;
  flex-wrap: wrap;
  flex-grow: 2;
  margin: 1rem;
  position: relative;
  z-index: 1;
}

.content-card:hover > .card-detail {
  display: flex;
  flex-direction: column;
  background: #d14646;
  z-index: 2;
  justify-content: center;
  align-items: center;
}
.content-card:last-child > .card-detail {
  display: flex;
  flex-direction: column;
  background: #d14646;
  z-index: 2;
  justify-content: center;
  align-items: center;
}
.card-img {
  max-width: 100%;
  height: auto;
}

.card-detail {
  position: absolute;
  display: none;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  padding: 1rem;
  border: 0.55rem solid white;
}
.detail-title {
  text-align: center;
  font-size: 2rem;
  position: relative;
  color: white;
  padding: 1rem;
}
.card-img-wrapper {
  display: flex;
  justify-content: center;
  align-content: center;
}
.detail-body {
  font-size: 1.25rem;
  padding: 1rem 0;
  color: white;
}
.detail-links {
  font-size: 3.25rem;
  display: flex;
  justify-content: center;
}
/* Portrait */
@media only screen and (min-device-width: 320px) and (max-device-width: 1023px) {
  .content::after {
    content: "";
    top: -15.85rem;
    left: -36rem;
    transform: rotate(145deg);
    position: absolute;
    padding: 35rem 35rem;
    background: #d14646;
  }
}
</style>