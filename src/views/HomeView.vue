<template>
  <section id="home" class="home">
    <main class="main-page">
      <div class="text">
        <h3>
          Hello there !
          <br />
          I'm
        </h3>
        <h1>KEREN BRUCE</h1>
        <br />
        <p>
          I build <span class="text--desc">elegant</span>,
          <span class="text--desc">reliable</span> and
          <span class="text--desc">functional</span> websites for various
          companies and aspire to become a
          <span class="text--desc">full stack developer</span> .
        </p>
      </div>
      <div class="home--buttons">
        <a href="#projects"><button class="main--btn">My Projects</button></a>
        <a href="#resume"><button class="main--btn">My Resume</button></a>
      </div>
    </main>
  </section>
</template>

<script>
export default {
  name: "HomeView",
  components: {},
};
</script>

<style scoped>
*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  overflow-x: hidden;
  flex-wrap: wrap;
  font-family: monospace;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 100%;
}

/* ----- Landing Page ----- */

.home {
  top: 6%;
  left: 0;
  right: 0;
  bottom: 0;
  width: 100%;
  position: absolute;
  overflow: hidden;
  padding: 8%;
  color: #ea638c;
  background-image: url("../assets/pink-flower-girl.png");
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: 44%;
  background-position-x: right;
  background-position-y: center;
}

.text {
  text-align: left;
  font-size: 2rem;
  font-weight: bold;
}

.text h1 {
  font-size: 5rem;
  font-weight: bolder;
  /*line-weight:;*/
  /*margin-left: -10px;*/
  color: transparent;
  -webkit-text-stroke: 1px #890230;
  background-image: url("../assets/favpng_rose-flower-pattern.png");
  -webkit-background-clip: text;
  background-position: 0 0;
  animation: back 20s linear infinite;
}

@keyframes back {
  100% {
    background-position: 2000px 0;
  }
}

.text p {
  font-size: 1.2rem;
}

.text--desc {
  font-size: 1.25rem;
  color: #890230;
  font-style: italic;
}

/* ----- Buttons on Landing Page ----- */

.home--buttons {
  margin-top: 0;
  margin-bottom: 0;
  padding: 2%;
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: center;
}

.home--buttons a {
  width: 35%;
  bottom: 0;
}

.main--btn {
  padding: 2%;
  width: 35%;
  background-color: #ffd9da;
  color: #89023e;
  font-size: 1.25rem;
  font-weight: bold;
  border-radius: 0.5rem;
}

.main--btn:hover,
.main--btn:focus {
  color: #ffd9da;
  background-color: #89023e;
  border: 2.5px solid #ffd9da;
}
</style>
