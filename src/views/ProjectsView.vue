<template>
  <MyProducts />
</template>

<script>
import MyProducts from "@/components/MyProducts.vue"
export default {
  name: "ProjectsView",
  components : {
    MyProducts
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
  margin: 10%;
  padding: 5%;
  box-sizing: border-box;
  overflow-x: hidden;
}
</style>
