<template>
  <div class="container">
    <div class="content"></div>
  </div>
</template>

<script>
export default {
  name: "Projects",
  data() {
    return {};
  },
  methods: {
    callProjects: function () {
      fetch("https://api.github.com/users/HermitRhaps/repos")
        .then((response) => response.json())
        .then((data) => console.log(data));
    },
  },
};
</script>

<style scoped>
.container {
  height: 100vh;
}
</style>