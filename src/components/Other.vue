<template>
  <div id="other">
    <div class="container">
      <div class="body">
        <div class="terminal">
          <div class="terminal-buttons">
            <div class="button-exit" />
            <div class="button-minimize" />
            <div class="button-fullscreen" />
          </div>
          <div class="terminal-body">
            <div class="request"><span>status</span></div>
            <div class="results">
              <div class="result"><span>😎</span></div>
            </div>
            <div class="request"><span>ls</span></div>
            <div class="results">
              <div class="result"><span>knowledge</span></div>
              <div class="result"><span>github</span></div>
              <div class="result"><span>linkedin</span></div>
            </div>
            <div class="request"><span>cd knowledge</span></div>
            <div class="request"><span>ls</span></div>
            <div class="results">
              <div class="result"><span>CSS.css</span></div>
              <div class="result"><span>HTML.html</span></div>
              <div class="result"><span>SQL&ORM.sql</span></div>
              <div class="result"><span>NodeJS.js</span></div>
              <div class="result"><span>PureJS.js</span></div>
              <div class="result"><span>React.jsx</span></div>
              <div class="result"><span>GitHub.git</span></div>
            </div>
            <div class="request"><span>cd -</span></div>
            <div class="request"><span>cd github</span></div>
            <div class="request"><span>ls</span></div>
            <div class="results">
              <div class="result"><span>link.exe</span></div>
            </div>
            <div class="request"><span>open link.exe</span></div>
            <div class="results">
              <div class="result">
                <a href="https://github.com/HermitRhaps"
                  >https://github.com/HermitRhaps</a
                >
              </div>
            </div>
            <div class="request"><span>cd -</span></div>
            <div class="request"><span>cd linkedin</span></div>
            <div class="request"><span>ls</span></div>
            <div class="results">
              <div class="result"><span>link.exe</span></div>
            </div>
            <div class="request"><span>open link.exe</span></div>
            <div class="results">
              <div class="result">
                <a href="https://www.linkedin.com/in/dmitry-nemov-8659a41a6/"
                  >https://www.linkedin.com/in/dmitry-nemov-8659a41a6/</a
                >
              </div>
            </div>
            <div class="request"><span>exit</span></div>
            <div class="results">
              <div class="result">
                <span>Bye!</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Other",
};
</script>

<style scoped>
.body {
  width: 100vw;
  height: 100vh;
  padding: 2vw;
}
.terminal {
  background-color: rgb(30, 30, 36);
  width: 100%;
  height: 100%;
  border-radius: 0.35vw;
  position: relative;
}
.terminal-buttons {
  padding: 0 1vh;
  width: 100%;
  height: 5vh;
  border-bottom: 0.45vh solid rgb(236, 238, 233);
  display: flex;
  align-items: center;
  justify-content: flex-start;
}
.button-exit {
  width: 5%;
  border-radius: 50%;
  width: 1.5vw;
  height: 1.5vw;
  background-color: red;
  margin: 0 0.35vh;
}
.button-minimize {
  width: 5%;
  border-radius: 50%;
  width: 1.5vw;
  height: 1.5vw;
  background-color: yellow;
  margin: 0 0.35vh;
}
.button-fullscreen {
  width: 5%;
  border-radius: 50%;
  width: 1.5vw;
  height: 1.5vw;
  background-color: green;
  margin: 0 0.35vh;
}
.terminal-body {
  padding: 1vw;
  color: white;
  font-size: 1.5vw;
}
.request::before {
  content: "~";
  margin: 0 0.65vw;
  color: yellowgreen;
}
.results {
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: flex-start;
}
.result {
  min-width: 5vw;
  margin: 0 1vh;
}
.result > a {
  color: green;
}
.result > a:hover {
  color: yellow;
}
@media only screen and (min-device-width: 320px) and (max-device-width: 1023px) {
  .terminal-body {
    font-size: 4.5vw;
  }
  .results {
    flex-wrap: wrap;
  }
}
</style>