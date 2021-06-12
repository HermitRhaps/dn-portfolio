<template>
  <nav class="navbar">
    <div class="navbar-item-logo">
      <a href="https://github.com/HermitRhaps" class="logo">
        <img src="../assets/logo.svg" alt="DN logo" />
      </a>
    </div>
    <div class="navbar-item-links">
      <ul
        class="nav-links"
        v-bind:class="{
          showed: isLinksShowed,
        }"
      >
        <li class="nav-link-item">About</li>
        <li class="nav-link-item">Projects</li>
        <li class="nav-link-item">Talk with me</li>
      </ul>
      <div
        class="nav-button"
        v-bind:class="{
          clicked: isLinksShowed,
        }"
        v-on:click="menuClick"
      >
        <div class="bar1" />
        <div class="bar2" />
        <div class="bar3" />
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return {
      isLinksShowed: false,
    };
  },
  methods: {
    menuClick: function () {
      this.isLinksShowed = !this.isLinksShowed;
    },
  },
};
</script>


<style scoped>
.navbar {
  width: 100%;
  display: flex;
  justify-content: space-between;
  padding: 0.25rem 0.75rem;
  background: #131116;
  color: white;
}

.nav-button {
  min-width: 5%;
  display: flex;
  flex-direction: column;
  align-items: center;
  cursor: pointer;
}

.navbar-item-logo {
  min-width: 5%;
  height: auto;
}
.navbar-item-links {
  min-width: 70%;
  display: flex;
  align-items: center;
  justify-content: flex-end;
}
/* menu-button  */
.bar1,
.bar2,
.bar3 {
  width: 2rem;
  height: 0.2rem;
  background: white;
  transition: 0.3s;
  margin: 0.15rem 0;
}
.clicked .bar1 {
  transform: rotate(-45deg) translate(0, 0.65rem);
}
.clicked .bar2 {
  opacity: 0;
}
.clicked .bar3 {
  transform: rotate(45deg) translate(0, -0.75rem);
}
.nav-links {
  min-width: 35%;
  display: flex;
  justify-content: space-around;
  align-items: center;
  opacity: 0;
  transition: 0.4s;
  cursor: pointer;
}
.nav-link-item {
  min-width: 1rem;
}
.nav-link-item:hover {
  color: rgb(219, 183, 136);
}
.showed {
  opacity: 1;
}
</style>
