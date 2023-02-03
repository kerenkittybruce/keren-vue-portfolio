<template>
  <div class="container">
    <div class="proj-intro">
      <h1 class="proj-title">Projects 🖤</h1>
      <br />
      <p class="proj-paragraph">
        <b
          >I would love to develop games, as well as useful web applications and
          software.</b
        >
        <em
          >I have worked on websites, portfolios, web applications and utility
          sites.</em
        >
        <b
          >I am looking to work alongside gaming companies to further enhance my
          skills and capabilities, while providing efficient, captivating and
          highly recommended user experience.</b
        >
        Here is a list of some projects I have completed :
      </p>
    </div>
    <div
      class="proj-card"
      v-for="(item, index) in myProjectsData.myProjects"
      :key="item"
    >
      <h2>{{ myProjectsData.myProjects[index].title }}</h2>
      <img
        class="proj-img"
        :src="myProjectsData.myProjects[index].image"
        alt="project-image"
      />
      <p>
        {{ myProjectsData.myProjects[index].description }}
      </p>
      <div class="site-links">
        <a :href="myProjectsData.myProjects[index].link"
          ><img
            class="link-img"
            src="https://i.postimg.cc/bYKPtrRg/netlify.png"
            alt="site-link"
        /></a>
        <br />
        <a :href="myProjectsData.myProjects[index].github"
          ><img
            class="link-img"
            src="https://i.postimg.cc/8Cb9XPW2/github2.png"
            alt="github"
        /></a>
      </div>
    </div>
  </div>
</template>

<script>
import jsonData from "/Users/Admin/keren-portfolio/projects.json";
export default {
  name: "MyProjects",

  data() {
    return {
      myProjectsData: jsonData,
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style scoped>
.container {
  margin-top: 6%;
  width: 100%;
  min-height: 100vh;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  background-color: #ea638c;
  color: #ffd9da;
}

.proj-intro {
  margin: 1.5%;
  padding: 2%;
  width: 100%;
  color: #30343f;
  text-align: center;
}

.proj-title {
  font-size: 2rem;
}

.proj-paragraph {
  font-size: 1.5rem;
}

.proj-card {
  margin: 2%;
  padding: 2%;
  width: 65%;
  background-color: #89023fd7;
  border-radius: 2rem;
  box-shadow: rgba(0, 0, 0, 0.7) 0px 4px 8px;
}
.proj-img {
  width: 50%;
}

.proj-card p {
  flex-wrap: wrap;
}

.site-links {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}

.link-img {
  height: 2.25rem;
  width: 2.25rem;
  margin: 1.5%;
}

/* Media Queries */

@media only screen and (min-width: 720px) {
  .container {
    margin-top: 30%;
    margin-bottom: 30%;
    padding-top: 5%;
    padding-bottom: 5%;
  }

  .proj-intro {
    margin: 0.5%;
  }

  .proj-paragraph {
    font-size: 1rem;
  }

  .proj-card {
    width: 90%;
  }

  .proj-img {
    width: 88%;
  }
}
</style>
