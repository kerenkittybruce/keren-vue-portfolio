<template>
  <section id="contact" class="contact">
    <div class="form">
      <h1>Talk To Me . . . 💕</h1>
      <form action="mailto:kerenchelseabruce@gmail.com">
        <div class="fullname">
          <label for="fullName">Full Name :</label>
          <input
            type="text"
            id="fname"
            name="fullname"
            placeholder="What is your first name ?"
            required
          />
        </div>
        <div class="email">
          <label for="email">E-mail Address :</label>
          <input
            type="email"
            id="email"
            name="email"
            placeholder="Enter your e-mail address ."
            required
          />
        </div>
        <div class="message">
          <label for="message">Message :</label>
          <textarea
            id="subject"
            name="subject"
            rows="3.85"
            cols="8"
            placeholder="What's on your mind ? Tell me and I'll respond to you as soon as possible ."
          ></textarea>
        </div>
        <div class="submit">
          <button type="submit">Submit</button>
        </div>
      </form>
    </div>
  </section>
</template>

<script>
export default {
  name: "ContactForm",

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
  overflow: hidden;
}

.contact {
  background-image: url("https://i.postimg.cc/13sghJ2L/favpng-rose-flower-pattern.png");
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;
  padding: 7%;
  width: 100%;
  /* min-height: 100vh; */
}

.contact h1 {
  color: #ea638e;
  font-size: 3rem;
  padding-bottom: 3%;
}

.form {
  margin: 0%;
  display: block;
  margin-left: auto;
  margin-right: auto;
  margin-bottom: 0%;
  width: 60%;
  padding: 3%;
  background-color: #89023e;
  flex-wrap: wrap;
}

input,
textarea {
  padding: 2%;
  margin: 2%;
  width: 90%;
  border: 2px solid #ea638e;
  border-radius: 2px;
  background-color: #ffd9da;
  box-sizing: border-box;
  resize: vertical;
}

label {
  margin: 2%;
  padding: 2%;
  color: #ffd9da;
  text-align: center;
  font-weight: bold;
  font-size: 1.3rem;
}

button {
  border: 2px solid #ffd9da;
  background-color: #89023e;
  color: #ffd9da;
  border-radius: 2px;
  font-weight: bold;
  margin-top: 2.5%;
  padding: 1.8%;
  width: 30%;
  font-size: 1rem;
}

button:hover {
  border: 2px solid #89023e;
  border-radius: 2px;
  background-color: #ffd9da;
  color: #89023e;
}
</style>
