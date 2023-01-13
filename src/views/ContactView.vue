<template>
  <HeaderComponent />
  <Form />
  <FooterComponent />
</template>

<script>
import HeaderComponent from "@/components/Header.vue";
import Form from "@/components/Form.vue";
import FooterComponent from "@/components/Footer.vue";
export default {
  name: "ContactView",
  components: {
    HeaderComponent,
    Form,
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
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  overflow-x: hidden;
  background-image: url("../assets/favpng_rose-flower-pattern.png");
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;
}
</style>
