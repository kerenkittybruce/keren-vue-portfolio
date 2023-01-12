<template>
  <div class="container">
    <div
      class="proj-card"
      v-for="(item, index) in myProjectsData.myProjects"
      :key="items"
    >
      <h2>{{ myProjectsData.myProjects[index].title }}</h2>
      <img :src="myProjectsData.myProjects[index].image" alt="product-image" />
      <p>{{ myProjectsData.myProjects[index].description }}</p>
      <div class="site-links">
        <a :href="myProjectsData.myProjects[index].firebase"
          ><img src="" alt="firebase"
        /></a>
        <a :href="myProjectsData.myProjects[index].github"
          ><img src="" alt="github"
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

<style scoped></style>
