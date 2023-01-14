<template>
  <HeaderComponent />
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
          <div class="link github" style="flex: 1">
            <img src="https://i.postimg.cc/8Cb9XPW2/github2.png" alt="github" />
            <a href="https://github.com/kerenkittybruce/kerenkittybruce"
              ><h3>Github</h3></a
            >
          </div>
          <div class="link" style="flex: 2">
            <img
              src="https://i.postimg.cc/8c39FMyh/pngegg-69.png"
              alt="twitter"
            />
            <a href="https://twitter.com/home?lang=en"><h3>Twitter</h3></a>
          </div>
          <div class="link" style="flex: 3">
            <img
              src="https://i.postimg.cc/43gCbvXP/pngegg-70.png"
              alt="LinkedIn"
            />
            <a href="https://www.linkedin.com/feed/"><h3>LinkedIn</h3></a>
          </div>
          <div class="link" style="flex: 4">
            <img
              src="https://i.postimg.cc/8c5gf1TV/pngegg-72.png"
              alt="Instagram"
            />
            <a href="https://www.instagram.com/kerenkittybruce/"
              ><h3>Instagram</h3></a
            >
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
  margin: 0;
  padding: 0;
  overflow-x: hidden;
  box-sizing: content-box;
  flex-wrap: wrap;
  font-family: monospace;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

section {
  background-image: url("https://i.postimg.cc/B6cyyZFW/Pngtree-high-grade-black-jewelry-luxurious-929300.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;
  margin: 7.75%;
  padding: 5%;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
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
  width: 35%;
  border-right: 2px solid #ffd9da;
  justify-content: center;
  align-items: center;
}

.profile img {
  width: 50%;
  border-radius: 50%;
}

.social-media {
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
  flex-wrap: wrap;
}

.link a {
  text-decoration: none;
  color: #ffd9da;
  font-size: 12px;
}

.link img {
  margin: 2%;
  padding: 2%;
  height: 3rem;
  width: 3rem;
  background-color: #ffd9da;
  border-radius: 50%;
}

.abt-desc {
  flex: 2;
  margin-top: 4%;
  width: 65%;
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
