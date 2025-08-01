<script>
import Header from "../src/components/Header.vue";
export default {
  //   data() {
  //     return {
  //       awesome: false,
  //     };
  //   },
  //   methods: {
  //     toggle(value) {
  //       this.awesome = value;
  //     },
  //   },

  components: {
    Header,
  },
};
</script>

<template>
  <Header />
  <!-- <div v-if="awesome">
    <h1>P</h1>
    <h1>o</h1>
    <h1>l</h1>
    <h1>o</h1>
    <h1>k</h1>
  </div> -->

  <!-- <div>
    <div>
      <h1 v-if="awesome === 'Polok'">Polok is Awesome!</h1>
      <h1 v-else-if="awesome === 'Banik'">Banik is Awesome!</h1>
      <h1 v-else>Vue is Super!</h1>
    </div>
    <button @click="toggle">Toggle</button>
  </div> -->
</template>

<style scoped></style>
