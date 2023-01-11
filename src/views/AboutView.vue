<template>
  <section id="about" class="about">
    <div class="profile">
      <img
        src="../assets/profile-placeholder-female.png"
        alt="profile-picture"
      />
      <div class="profile-txt">
        <h1>Keren Chelsea Bruce</h1>
        <p>Software Developer</p>
      </div>
    </div>
    <div class="abt-desc">
      <p class="aboutme-1">
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
      <p class="aboutme-2">
        I am a full-stack web developer and designer, as well as a cloud
        practitioner for Amazon Web Services (AWS). I build high quality
        websites and web applications that are captivating and exciting, yet
        radiate boss levels. I always adhere to my clients' specifications and
        desires while showcasing my skills in a fascinating way. I'm a fast
        learner and love to build on the skills and knowledge I already have, so
        if you feel there is any way for me to improve, please let me know.
      </p>
    </div>
  </section>
</template>

<script>
export default {
  name: "AboutView",

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
  font-family: monospace;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
section {
  margin: 8%;
  padding: 5%;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
}

.profile,
.abt-desc {
  background-color: rgba(137, 2, 47, 0.912);
  color: #ffd9da;
  padding: 2.5%;
  font-size: large;
  font-weight: bold;
}

.profile {
  flex: 1;
  width: 35%;
  border-right: 2px solid #ffd9da;
}

.profile img {
  width: 50%;
  border-radius: 50%;
}

.abt-desc {
  flex: 2;
  width: 65%;
}
</style>
