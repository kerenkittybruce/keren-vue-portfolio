<template>
  <HeaderComponent />
  <div class="t-page">
    <p class="title">What People Are Saying . . 💗</p>
    <div class="testimonials">
      <div class="t-card" v-for="test in testimonials" :key="test">
        <img :src="test.image" alt="display-image">
        <p class="t-name" v-text="test.name"></p>
        <br />
        <p class="t-role" v-text="test.role"></p>
        <br />
        <p class="t-quote" v-text="test.quote"></p>
      </div>
    </div>
  </div>
  <FooterComponent />
</template>

<script>
import HeaderComponent from "@/components/Header.vue";
import FooterComponent from "@/components/Footer.vue";
export default {
  name: "TestimonialsView",
  components: {
    HeaderComponent,
    FooterComponent,
  },

  data() {
    return {
      testimonials: [
        {
          id: 1,
          name: "💗 Candice Amon 💗",
          role: "Facilitator -- Life Choices Coding Academy",
          quote:
            "Keren has a very professional and mature approach and outlook on life. Values healthy relationships and show tremendous respect to whoever she encounters. She believes in working hard for what she wants and knows when to make sacrifices in order to succeed.",
        },
        {
          id: 2,
          name: "💗 Oslin Johnson 💗",
          role: "Lecturer -- Life Choices Coding Academy",
          quote:
            "Keren is a soft soul but, very determined and driven to be the best creative she can be. Her soft nature makes her a joy to work with and give good advice knowing that she will put her best foot forward in every situation.",
        },
        {
          id: 3,
          name: "💗 Mishaine Isaacs 💗",
          role: "Colleague -- Life Choices Coding Academy",
          quote:
            "She works well under pressure and loves learning. She is highly motivated and produces elegant projects which showcase her skills accurately. She is lovely to work with, especially in a team setting. Her beautiful creativity and exceptional work ethic will ensure that your reputation keeps improving.",
        },
        {
          id: 4,
          name: "💗 Sadia Alam 💗",
          role: "Former Colleague -- Life Choices Coding Academy",
          quote:
            "Keren is a very kind and intelligent individual. She is a very quick learner and has good problem solving skills. Keren has a passion for programming and only produces quality products. She would be quite the asset to have in any company.",
        },
        {
          id: 5,
          name: "💗 Abdul Azeez - Kemp 💗",
          role: "Colleague -- Life Choices Coding Academy",
          quote:
            "Keren is a wonderful lady, personality is one of kind, unique. Hard working individual and great to work with and always available with a smile on her face if you need assistance or to just to conversate with. And she will always put a smile on your, all-in-all, she'll be a wonderful person to be in your company.",
        },
        {
          id: 6,
          name: "💗 Xolelwa Manqina 💗",
          role: "Colleague -- Life Choices Coding Academy",
          quote:
            "Keren is a hard working lady. She is organised , efficient and extremely competent with excellent rapport with people of all ages. Her communication skills are excellent no matter if you are talking about verbal or written. Her most important quality is that she always keeps herself updated with new information. Its just amazing to work with such a kind personality. I highly recommend Keren Bruce for any position or endeavor that she may pursue. She would be a valueable asset to your company.",
        },
      ],
    };
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
}

.t-page {
  background-color: #1b2021;
  color: #ffd9da;
  margin-top: 8%;
  margin-bottom: 6.9%;
  padding: 3%;
  font-weight: bold;
  display: flex;
  flex-wrap: wrap;
  background-image: url("../assets/cherry-fragments.png");
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover;
  background-position-x: right;
}

.title {
  background-color: #1b2021d2;
  border-radius: 2.5%;
  width: 70%;
  padding: 2%;
  color: #ea638e;
  font-size: 2.95rem;
  margin-left: auto;
  margin-right: auto;
}

.t-card {
  border: 1.56px solid #ffd9da;
  box-shadow: 0 4px 8px 0 #1b2021;
  border-radius: 2rem;
  margin: 5%;
  padding: 3%;
  background-color: #1b2021d2;
}

.t-name {
  color: #ea638e;
  font-size: 2rem;
}

.t-role {
  font-size: 1.3rem;
}

.t-quote {
  font-size: 1rem;
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 80%;
}
</style>
