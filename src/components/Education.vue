<template>
  <div id="education">
    <div class="container">
      <div class="header">
        <div class="icon">
          <img src="../assets/card-icon.svg" alt="icon" />
        </div>
        <div class="detail">
          <span>Education.</span>
        </div>
        <a href="#about">
          <div class="up">
            <img src="../assets/arrow-down.svg" alt="arrow" />
          </div>
        </a>
        <div class="down">
          <img src="../assets/arrow-down.svg" alt="arrow" />
        </div>
      </div>
      <div class="body">
        <div class="graph">
          <div class="initial" />
          <div class="middle">Software Engineer</div>
          <div class="end">Student lab</div>
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
  name: "Education",
};
</script>

<style scoped>
.header {
  background-image: url("../assets/education.jpeg");
}
.graph {
  font-size: 5vh;
}
.initial,
.middle,
.end {
  font-size: 3vh;
}
.initial,
.middle {
  position: relative;
}
.initial::before {
  content: "School";
  display: flex;
  font-size: 5vh;
}
.middle::before {
  content: "BNTU";
  display: flex;
  font-size: 5vh;
}
.end::before {
  content: "TeachMeSkill";
  display: flex;
  font-size: 5vh;
}
.initial::after,
.middle::after {
  content: "";
  display: block;
  position: relative;
  width: 0.4vw;
  height: 10vh;
  left: 5vh;
  background: black;
}
</style>