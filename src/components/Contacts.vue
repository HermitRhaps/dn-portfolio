<template>
  <div id="contacts">
    <div class="container">
      <div class="header">
        <div class="part-h" />
        <div class="contact-form">
          <p class="line contact-type">
            <a href="mailto: hermitrequiem@gmail.com">Contact me for more.</a>
          </p>
        </div>
      </div>
      <div class="content">
        <div class="part-c" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Contacts",
};
</script>

<style scoped>
.header {
  width: 75vw;
  position: relative;
}
.content {
  width: 25vw;
  position: relative;
}
.part-h {
  content: "1";
  display: block;
  position: absolute;
  width: 100rem;
  height: 100rem;
  padding: 1rem;
  transform: rotate(-45deg);
  background-color: rgb(30, 30, 36);
  left: 0;
  bottom: -50rem;
}
.part-c {
  content: "1";
  display: block;
  position: absolute;
  width: 120rem;
  height: 100rem;
  padding: 1rem;
  transform: rotate(45deg);
  background-color: rgb(30, 30, 36);
  left: -31rem;
  top: -58rem;
}

.contact-form {
  position: absolute;
  padding: 1rem;
  bottom: 0;
  left: 0;
}
.line {
  white-space: nowrap;
  overflow: hidden;
  border-right: 0.45rem solid rgba(255, 255, 255, 0.75);
  font-size: 5rem;
  animation: typing 2s steps(22), blink 0.5s step-end infinite alternate;
  border-right: 3px solid;
  width: 17.5ch;
  color: white;
}
.line > a {
  color: white;
}

@keyframes typing {
  from {
    width: 0;
  }
}
@keyframes blink {
  50% {
    border-color: transparent;
  }
}

@media only screen and (min-device-width: 320px) and (max-device-width: 1023px) {
  .part-h {
    display: none;
  }
  .part-c {
    left: -2.1rem;
    top: -50rem;
    transform: rotate(25deg);
  }
  .line {
    font-size: 2.4rem;
    color: rgb(30, 30, 36);
  }
  .line > a {
    color: rgb(30, 30, 36);
  }
}
</style>