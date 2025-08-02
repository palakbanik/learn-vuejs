<template>
  <h1>Simple Form</h1>

  <form action="">
    <label for="email">Email: </label>
    <input
      type="email"
      id="email"
      placeholder="enter email.."
      autocomplete="current-email"
      ref="emailInput"
      v-model="form.email"
    />
    <br /><br />

    <label for="password">Password: </label>
    <input
      type="password"
      id="password"
      placeholder="enter password..."
      autocomplete="current-password"
      ref="passwordInput"
      v-model="form.password"
    />
    <br /><br />

    <select name="" id="" v-model="form.country">
      <option value="bangladesh" selected>Bangladesh</option>
      <option value="india">India</option>
      <option value="usa">USA</option>
      <option value="chine">Chine</option>
    </select>

    <br /><br />

    <button @click="getValue" type="submit">Login</button>
  </form>

  <p>Email is: {{ form.email }}</p>
  <p>Password is: {{ form.password }}</p>
  <p>Country is: {{ form.country }}</p>
  <p>Technology is: {{ form.technology }}</p>
  <p>Gender is: {{ form.gender }}</p>
</template>

<script>
export default {
  name: "SimpleForm",

  data() {
    return {
      form: {
        email: "",
        password: "",
        country: "",
        technology: "",
        gender: "",
      },
    };
  },

  methods: {
    getValue(e) {
      e.preventDefault();
      this.email = this.$refs.emailInput.value;

      console.log(this.$refs.emailInput.value);
      console.log(this.$refs.passwordInput.value);
    },
  },
};
</script>

<style></style>
