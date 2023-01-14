<template>
  <HeaderComponent />
  <ResumeInfo />
  <FooterComponent />
</template>

<script>
import HeaderComponent from "@/components/Header.vue";
import ResumeInfo from "@/components/Resume.vue";
import FooterComponent from "@/components/Footer.vue";
export default {
  name: "ResumeView",
  components: {
    HeaderComponent,
    ResumeInfo,
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
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
