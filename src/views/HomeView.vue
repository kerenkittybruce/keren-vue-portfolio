<template>
  <HeaderComponent />
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
          companies
          <br />
          and aspire to become a
          <span class="text--desc">full stack developer</span> .
        </p>
      </div>
    </main>
  </section>
  <FooterComponent />
</template>

<script>
import HeaderComponent from "@/components/Header.vue";
import FooterComponent from "@/components/Footer.vue";
export default {
  name: "HomeView",
  components: {
    HeaderComponent,
    FooterComponent,
  },
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
  top: 5.75%;
  left: 0;
  right: 0;
  bottom: 0;
  width: 100%;
  min-height: 100vh;
  overflow: hidden;
  padding: 8%;
  color: #ffd9da;
  background-color: #30343f;
  background-image: url("../assets/pink-flower-girl.png");
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: 44%;
  background-position-x: right;
  background-position-y: center;
}

.text {
  margin-top: 9.48%;
  text-align: left;
  font-size: 2rem;
  font-weight: bold;
}

.text h1 {
  font-size: 9.2rem;
  font-weight: bolder;
  color: transparent;
  -webkit-text-stroke: 1.05px #ffd9da;
  background-image: url("https://i.postimg.cc/13sghJ2L/favpng-rose-flower-pattern.png");
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
  color: #ea638e;
  font-style: italic;
}

/* Media Queries */

@media only screen and (max-width: 301px) {
  .main-page {
    margin-top: 3rem;
    width: 80%;
    padding: 1%;
    color: #ffd9da;
    background-color: #30343f;
    background-size: 90%;
  }
}
</style>
