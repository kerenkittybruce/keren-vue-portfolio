<template>
  <section id="resume" about="resume">
    <div class="tech-container">
      <div
        class="tech-card"
        v-for="(item, index) in myTechLearned.skills"
        :key="item"
      >
        <h2>{{ myTechLearned.skills[index].name }}</h2>
        <img :src="myTechLearned.skills[index].image" alt="tech-logo" />
        <p>{{ myTechLearned.skills[index].description }}</p>
      </div>
    </div>
  </section>
</template>

<script>
import jsonData from "@/components/Resume.vue";
export default {
  name: "ResumeInfo",

  data() {
    return {
      myTechLearned: jsonData,
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style scoped>
.tech-container {
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

.tech-card img {
  height: 10rem;
}

.tech-card {
  margin: 2%;
  display: flex;
  flex-wrap: 0 0 45%;
  background-color: #89023e;
  border-radius: 2rem;
  box-shadow: rgba(0, 0, 0, 0.7) 0px 4px 8px;
  padding: 2%;
}
</style>
