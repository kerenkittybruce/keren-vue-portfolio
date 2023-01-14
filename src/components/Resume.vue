<template>
  <div class="container">
    <div class="res-intro">
      <h1 class="res-title">Resume 🖤</h1>
      <br />
      <hr />
      <br />
      <h2 class="res-skills">Skills :</h2>
      <p class="res-paragraph">
        🖤 I am a creative, ambitious software developer with an intense craving
        to gain experience designing and developing user-centered material from
        initial concept to finish, to the best of my ability. 🖤
        <br />
        🖤 I am happy to learn more , despite skills and capablities I have
        obtained already . 🖤
        <br />
        Here is a list of some skills I have obtained :
      </p>
    </div>
    <div
      class="res-card"
      v-for="(item, index) in myResData.mySkills"
      :key="item"
    >
      <h2>{{ myResData.mySkills[index].name }}</h2>
      <img
        class="res-img"
        :src="myResData.mySkills[index].image"
        alt="resume-image"
      />
      <p>
        {{ myResData.mySkills[index].description }}
      </p>
    </div>
    <br />
    <div class="work">
      <p class="wrk-p">
        🖤 I enjoy working with people, especially those who are open-minded and
        passionate about their work . I love learning from them, as well as
        guiding them towards their aspirations . 🖤
        <br />
        🖤🖤 My Journey So Far : 🖤🖤
      </p>
      <br />
      <div class="work-exp">
        <div class="wrk-01">
          <h2>Empire Promotions</h2>
          <p class="position">Promoter</p>
          <p class="duration">26/01/2018 - 15/04/2018</p>
          <br />
          <h3>Responsibilities</h3>
          <ul>
            <li>
              Demonstrate and provide information on promoted products /
              services.
            </li>
            <li>Create a positive image and lead customers to use it.</li>
            <li>
              Identify interest and understand customer needs and requirements.
            </li>
            <li>Use tasting samples in order to receive feedback.</li>
          </ul>
        </div>
        <div class="wrk-02">
          <h2>Game - Canal Walk</h2>
          <p class="position">Gift Wrapper / Cashier</p>
          <p class="duration">15/11/2019 - 31/12/2019</p>
          <br />
          <h3>Responsibilities</h3>
          <ul>
            <li>Wrapping fragile items in order to ensure safe transport.</li>
            <li>
              Asking customers for the correct amount of money, and taking
              payment by cash / credit.
            </li>
            <li>Issue receipts, refunds, change or tickets.</li>
            <li>Redeem stamps, coupons or certificates.</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import jsonData from "/Users/Admin/keren-portfolio/projects.json";
export default {
  name: "MyProjects",

  data() {
    return {
      myResData: jsonData,
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style scoped>
.container {
  margin-top: 6%;
  margin-bottom: 4.5%;
  width: 100%;
  min-height: 100vh;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  background-color: #ea638c;
  color: #ffd9da;
  font-weight: bold;
  background-image: url("https://i.postimg.cc/wBFjpzLN/abstractpinkpaint.jpg");
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover;
}

.res-intro {
  margin: 1.5%;
  padding: 2%;
  width: 100%;
  color: #30343f;
  text-align: center;
}

.res-title {
  font-size: 2rem;
}

.res-skills {
  font-size: 1.5rem;
}

.res-paragraph {
  font-size: 1.3rem;
}

.res-card {
  margin: 2%;
  padding: 2%;
  width: 65%;
  background-color: #89023e;
  border-radius: 2rem;
  box-shadow: rgba(0, 0, 0, 0.7) 0px 4px 8px;
}
.res-img {
  width: 50%;
}

.res-card p {
  flex-wrap: wrap;
}

hr {
  color: #ea638c;
}

.work {
  background-color: #ffd9da;
  color: #89023e;
  margin-bottom: 6%;
  padding: 2%;
  font-weight: bold;
}

.wrk-p {
  font-size: 1.5rem;
}

.work-exp {
  margin-left: 2%;
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  flex-wrap: wrap;
  align-items: center;
}

.wrk-01 {
  flex: 1;
  width: 50%;
  padding: 2%;
  margin-bottom: 2%;
  border: 3px solid #89023e;
  border-radius: 2rem;
  background: opacity 0.8;
}

.wrk-02 {
  flex: 2;
  width: 50%;
  padding: 2%;
  border: 3px solid #89023e;
  border-radius: 2rem;
  background: opacity 0.8;
}

.work-exp h2 {
  font-size: 1.375rem;
}

.position {
  font-size: 1.15rem;
}

.duration {
  font-size: 0.9rem;
}
</style>
