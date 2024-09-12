<template>
  <h1>Contact us</h1>
  <form v-on:submit.prevent="greetUser">
    <label for="username">Username:</label>
    <input type="text" v-model="username" />

    <br />
    <label for="useremail">Email:</label>
    <input type="text" v-model="useremail" />

    <br />
    <label for="Message">Message:</label>
    <input type="text" v-model="usermessage" />

    <br />

    <button type="submit">Send Message</button>
  </form>

  <h1>results</h1>
  <h2>{{ username }}</h2>
  <h2>{{ useremail }}</h2>
  <h2>{{ usermessage }}</h2>
</template>

<script>
export default {
  name: "ContactUs",
  data() {
    return {
      username: "",
      useremail: "",
      usermessage: "",
    };
  },
  methods: {
    greetUser() {
      alert(
        `Hello ${this.username} with the email ${this.useremail} your message has been sent successfully`
      );
    },
  },
};
</script>

<style scoped>
h1 {
  text-align: center;
  color: blue;
}
</style>
