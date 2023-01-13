<template>
  <div class="footer">
    <h2>ⓒ Keren Chelsea Bruce 2023 | All Rights Reserved .</h2>
  </div>
</template>

<script>
export default {
  name: "FooterComponent",

  data() {
    return {};
  },

  mounted() {},

  methods: {},
};
</script>

<style scoped>
.footer {
  width: 100%;
  padding: 1%;
  background-color: #1b2021;
  color: #ffd9da;
  text-align: center;
  justify-content: center;
  overflow-x: hidden;
  position: fixed;
  left: 0;
  bottom: 0;
  font-family: monospace;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font-weight: bold;
}

.footer h2 {
  font-size: 0.85rem;
  font-weight: bold;
}
</style>
