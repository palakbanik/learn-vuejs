<script>
export default {
  data() {
    return {
      isUserLoggedIn: false,
    };
  },

  methods: {
    signIn() {
      this.isUserLoggedIn = true;
    },
    logout() {
      this.isUserLoggedIn = false;
    },
  },
};
</script>

<template>
  <header>
    <h1>POLOK</h1>

    <div v-if="!isUserLoggedIn">
      <button @click="signIn">SIGN IN</button>
      <button>SIGN UP</button>
    </div>

    <div v-else>
      <button>PROFILE</button>
      <button @click="logout">LOG OUT</button>
    </div>
  </header>
</template>

<style scoped></style>
