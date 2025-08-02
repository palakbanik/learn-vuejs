<template>
  <h1>Ref in Vue.js</h1>

  <div>
    <input type="text" ref="textInput" />
    <button @click="getInputField">Click here</button>
  </div>
</template>

<script>
export default {
  name: "Ref",

  methods: {
    getInputField() {
      this.$refs.textInput.focus();
      this.$refs.textInput.style.color = "blue";
      console.log(this.$refs.textInput.value);
    },
  },
};
</script>

<style></style>
