<template>
  <!-- <h1>hello world</h1> -->

  <h1>HTML Binding</h1>

  <div>{{ text }}</div>

  <div v-html="nameTag"></div>
  <div v-html="emailTag"></div>
</template>

<script>
export default {
  name: "HTMLBinding",
  data() {
    return {
      text: "Hello World",
      nameTag: "<h1>Polok Banik</h1>",
      emailTag: "<h1>polok@test.com</h1>",
    };
  },
};
</script>

<style></style>
