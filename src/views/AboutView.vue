<template>
  <HeaderComponent />
  <br />
  <section id="about" class="about">
    <div class="profile">
      <img
        src="https://i.postimg.cc/MTfJ71HK/IMG-2.jpg"
        alt="profile-picture"
      />
      <div class="profile-txt">
        <h1>Keren Chelsea Bruce</h1>
        <p>Software Developer</p>
        <div class="social-media">
          <div class="link github" style="flex: 1, width: 20%;">
            <a href="https://github.com/kerenkittybruce/kerenkittybruce"
              ><img
                src="https://i.postimg.cc/8Cb9XPW2/github2.png"
                alt="github"
            /></a>
          </div>
          <div class="link" style="flex: 2, width: 20%;">
            <a href="https://twitter.com/home?lang=en">
              <img
                src="https://i.postimg.cc/8c39FMyh/pngegg-69.png"
                alt="twitter"
            /></a>
          </div>
          <div class="link" style="flex: 3, width: 20%;">
            <a href="https://www.linkedin.com/feed/">
              <img
                src="https://i.postimg.cc/43gCbvXP/pngegg-70.png"
                alt="LinkedIn"
            /></a>
          </div>
          <div class="link" style="flex: 4, width: 20%;">
            <a href="https://www.instagram.com/kerenkittybruce/"
              ><img
                src="https://i.postimg.cc/8c5gf1TV/pngegg-72.png"
                alt="Instagram"
            /></a>
          </div>
        </div>
      </div>
    </div>
    <div class="abt-desc">
      <p style="padding-bottom: 3%">
        <b
          >I am a passionate and creative full-stack developer who enjoys
          working on projects and developing useful tools for people everywhere
          to benefit from.</b
        >
        <br />
        <em
          >I also enjoy gaming, listening to music, singing, dancing, and
          learning about various concepts including spirituality and psychology.
          I look forward to working with amazing energetic and positive
          people.</em
        >
        <br />
        <b
          >I currently live in Cape Town which is situated in Western Cape,
          South Africa</b
        >. I enjoyed doing Business Studies in high school, and now I have
        transitioned into doing coding projects for companies of various
        specialties.
      </p>
      <p style="padding-bottom: 3%">
        I am an aspiring full-stack web developer and designer, as well as a
        cloud practitioner for Amazon Web Services (AWS). I build high quality
        websites and web applications that are captivating and exciting, yet
        radiate boss levels. I always adhere to my clients' specifications and
        desires while showcasing my skills in a fascinating way. I'm a fast
        learner and love to build on the skills and knowledge I already have, so
        if you feel there is any way for me to improve, please let me know.
      </p>
      <p>
        I look forward to working with various people and in exciting new
        environments.
      </p>
    </div>
  </section>
  <br />
  <FooterComponent />
</template>

<script>
import HeaderComponent from "@/components/Header.vue";
import FooterComponent from "@/components/Footer.vue";
export default {
  name: "AboutView",
  components: {
    HeaderComponent,
    FooterComponent,
  },

  data() {
    return {};
  },

  mounted() {},

  methods: {},
};
</script>

<style scoped>
* {
  padding: 0;
  overflow-x: hidden;
  box-sizing: content-box;
  flex-wrap: wrap;
  font-family: monospace;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #30343f;
}

body {
  overflow-x: hidden;
  width: 100%;
  margin-top: 7%;
}

section {
  margin-top: 5%;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  background-color: #30343f;
  background-image: url("../assets/cherry-right.png");
  /*background-position-x: left;*/
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;
}

.profile,
.abt-desc {
  color: #ffd9da;
  padding: 2.5%;
  font-size: large;
  font-weight: bold;
}

.profile {
  flex: 1;
  margin-top: 5%;
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 30%;
  background-color: #ea638cb2;
  border: 0.5px solid #ea638c;
  border-radius: 2.5%;
  box-shadow: 0 4px 8px 0 #ea638c;
  border-bottom: 2px solid #ffd9da;
  justify-content: center;
  align-items: center;
}

.profile img {
  width: 40%;
  border-radius: 50%;
}

.profile-txt {
  border-radius: 2%;
}

.social-media {
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  margin: 5%;
}

.link {
  width: 20%;
}

.link a {
  text-decoration: none;
  color: #ffd9da;
  font-size: 12px;
}

.link img {
  padding: 2%;
  height: 2rem;
  width: 2rem;
  background-color: #ffd9da;
  border-radius: 50%;
}

.link img:hover {
  background-color: #ea638e;
  height: 1.8rem;
  width: 1.8rem;
}

.abt-desc {
  flex: 2;
  margin-top: 8%;
  margin-left: auto;
  margin-right: auto;
  margin-bottom: 6%;
  width: 50%;
  border-radius: 2.5%;
  justify-content: center;
  align-items: center;
}

/* Media Queries */

@media only screen and (max-width: 301px) {
  section {
    margin-top: 30%;
    margin-bottom: 30%;
    flex-direction: column;
    justify-content: center;
  }

  .profile {
    width: 95%;
    border-right: none;
    border-bottom: 2px solid #ffd9da;
  }

  .abt-desc {
    width: 95%;
  }

  .social-media {
    flex-direction: column;
  }

  .link img {
    height: 2rem;
    width: 2rem;
    margin: 4%;
    padding: 2%;
  }
}

@media only screen and (max-width: 720px) {
  section {
    margin-top: 12%;
    flex-direction: row;
    justify-content: center;
  }

  .profile {
    margin: 8%;
    padding: 4%;
    justify-content: center;
    align-content: center;
    width: 95%;
  }

  .profile img {
    width: 100%;
    margin-bottom: 3%;
    border-radius: 50%;
  }

  .abt-desc {
    width: 95%;
  }

  .social-media {
    padding: 6%;
    flex-direction: column;
  }

  .link img {
    height: 2rem;
    width: 2rem;
    margin: 30%;
    padding: 3%;
  }
}
</style>
