<template>
  <h1>Class Binding Component</h1>

  <h2 :class="{ green: colorFull }">Hello World</h2>
  <br />
  <br />
  <button @click="changeBg">Change Bg</button>
</template>

<script>
export default {
  name: "Class Binding",
  data() {
    return {
      colorFull: true,
    };
  },

  methods: {
    changeBg() {
      this.colorFull = !this.colorFull;
    },
  },
};
</script>

<style scoped>
.green {
  background: green;
  display: inline;
  padding: 5px;
}
</style>
