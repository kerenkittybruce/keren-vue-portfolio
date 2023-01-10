<template>
  <nav style="font-size: 1rem; text-decoration: none;">
    <router-link to="/">Home</router-link> 🖤
    <router-link to="/about">About</router-link> 🖤
    <router-link to="/skills">Skills</router-link> 🖤
    <router-link to="/testimonials">Testimonials</router-link> 🖤
    <router-link to="/resume">Resume</router-link> 🖤
    <router-link to="/contact">Contact</router-link>
  </nav>
</template>

<script>
export default {
  name: "NavbarComponent",

  data() {
    return {};
  },

  mounted() {},

  methods: {},
};
</script>

<style scoped>
nav {
  top: 0;
  left: 0;
  right: 0;
  padding: 2.5%;
  position: fixed;
  background-color: #ffd9da;
}

nav router-link {
  color: black;
}

nav a {
  font-weight: bold;
  color: black;
}

nav router-link:hover {
  color: #89023e;
  font-size: 1.5rem;
}

nav a.router-link-exact-active {
  color: #89023e;
}
</style>
