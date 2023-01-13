<template>
  <HeaderComponent />
  <MyProjects />
  <FooterComponent />
</template>

<script>
import HeaderComponent from "@/components/Header.vue";
import MyProjects from "@/components/MyProjects.vue";
import FooterComponent from "@/components/Footer.vue";
export default {
  name: "ProjectsView",
  components: {
    HeaderComponent,
    MyProjects,
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
  box-sizing: border-box;
  overflow-x: hidden;
  background-image: url("../assets/flower-decor.png");
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: contain;
  background-position-x: right;
  background-position-y: top;
}
</style>
