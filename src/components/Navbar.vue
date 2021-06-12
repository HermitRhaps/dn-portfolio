<template>
  <nav class="navbar">
    <a href="https://github.com/HermitRhaps" class="logo">
      <img src="../assets/logo.svg" alt="DN logo" />
    </a>

    <div class="nav-button">
      <div class="bar1" />
      <div class="bar2" />
      <div class="bar3" />
    </div>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
};
</script>


<style scoped>
.navbar {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0.25rem 0.75rem;
  background: #131116;
  color: white;
}
.logo {
  min-width: 5%;
  height: auto;
}
.nav-button {
  min-width: 5%;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.bar1,
.bar2,
.bar3 {
  width: 2rem;
  height: 0.2rem;
  background: white;
  transition: 0.4s;
  margin: 0.15rem 0;
}
</style>
