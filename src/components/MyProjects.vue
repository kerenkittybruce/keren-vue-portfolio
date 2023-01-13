<template>
  <div class="container">
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
          ><img src="../assets/netlify.png" alt="site-link"
        /></a>
        <br />
        <a :href="myProjectsData.myProjects[index].github"
          ><img class="github" src="../assets/github2.png" alt="github"
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
  margin-top: 5%;
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

.proj-card {
  margin: 2%;
  padding: 2%;
  background-color: #89023e;
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

.site-links img {
  height: 2rem;
  margin: 1.25%;
}

.github {
  padding-left: 0.5rem;
}
</style>
