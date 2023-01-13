<template>
  <section id="contact" class="contact">
    <div class="form">
      <h1>Talk To Me . . . 💕💕</h1>
      <form action="mailto:kerenchelseabruce@gmail.com">
        <div class="fullname">
          <label for="firstName">First Name :</label>
          <input
            type="text"
            id="fname"
            name="firstname"
            placeholder="What is your first name ?"
            required
          />
        </div>
        <div class="lastname">
          <label for="lastName">Last Name :</label>
          <input
            type="text"
            id="lname"
            name="lastname"
            placeholder="What is your last name ?"
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
            rows="5"
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
  overflow-x: hidden;
}

.contact {
  padding: 6%;
  width: 100%;
  min-height: 100vh;
}

.contact h1 {
  font-size: 3.25rem;
}

.form {
  top: 2.5%;
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 70%;
  padding: 3%;
  background-color: rgba(255, 217, 218, 0.873);
  flex-wrap: wrap;
}

input,
textarea {
  padding: 2%;
  width: 100%;
  border: 2px solid #89023e;
  border-radius: 2px;
  background-color: #ffd9da;
  box-sizing: border-box;
  resize: vertical;
}

label {
  margin: 2%;
  padding: 2%;
  color: #89023e;
  text-align: center;
  font-weight: bold;
  font-size: 1.25rem;
}

button {
  border: 2px solid #89023e;
  background-color: #89023e;
  color: #ffd9da;
  border-radius: 2px;
  font-weight: bold;
  padding: 2%;
}

button:hover {
  border: 2px solid #89023e;
  background-color: #ffd9da;
  color: #89023e;
}
</style>
