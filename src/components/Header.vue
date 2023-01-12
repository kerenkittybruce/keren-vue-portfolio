<template>
  <div class="header">
    <NavbarComponent />
  </div>
</template>

<script>
import NavbarComponent from "@/components/Navbar.vue";

export default {
  name: "HeaderComponent",
  components: {
    NavbarComponent,
  },

  data() {
    return {};
  },

  mounted() {},

  methods: {},
};
</script>

<style scoped>
.header {
  position: fixed;
  width: 100%;
  color: #1b2021;
  box-shadow: 0 4px 4px -4px rgba(0, 0, 0, 0.5);
}

</style>
