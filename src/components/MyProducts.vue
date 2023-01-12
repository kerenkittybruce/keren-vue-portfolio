<template>
  <div class="container">
    <div
      class="proj-card"
      v-for="(item, index) in myProjectsData.myProjects"
      :key="item"
    >
      <h2>{{ myProjectsData.myProjects[index].title }}</h2>
      <img :src="myProjectsData.myProjects[index].image" alt="product-image" />
      <p>{{ myProjectsData.myProjects[index].description }}</p>
      <div class="site-links">
        <a :href="myProjectsData.myProjects[index].link"
          ><img src="../assets/netlify.png" alt="site-link"
        /></a>
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
  name: "MyProducts",

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
}

.proj-card img {
  height: 10rem;
}

.proj-card {
  margin: 2%;
  flex-wrap: 0 0 45%;
  background-color: #89023e;
  border-radius: 2rem;
  box-shadow: rgba(0, 0, 0, 0.7) 0px 4px 8px;
  padding: 2%;
}

.site-links {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  align-items: center;
}

.site-links img {
  height: 1.5rem;
  margin: 1.25%;
}

/*.github{
    width: 100%;
}*/
</style>
