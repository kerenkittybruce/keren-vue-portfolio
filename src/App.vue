<template>
  <HeaderComponent />
  <FooterComponent />
  <router-view />
</template>

<script>
import HeaderComponent from "@/components/Header.vue";
import FooterComponent from "@/components/Footer.vue";

export default {
  name: "KerenPortfolioApp",
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

<style>
#app {
  font-family: monospace;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  flex-wrap: wrap;
}
</style>
