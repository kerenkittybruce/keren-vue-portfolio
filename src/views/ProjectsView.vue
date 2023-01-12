<template>
  <MyProducts />
</template>

<script>
import MyProducts from "@/components/MyProducts.vue";
export default {
  name: "ProjectsView",
  components: {
    MyProducts,
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
  padding: 5%;
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
