<template>
  <h1>Parent Component</h1>
  <br />

  <ul>
    <li v-for="user in users" :key="user.name">
      <Child :data="user" :getNameData="getNameData" />
    </li>
  </ul>
</template>

<script>
import Child from "./Child.vue";

export default {
  name: "Parent",

  methods: {
    getNameData(name) {
      alert(name);
    },
  },

  components: {
    Child,
  },

  data() {
    return {
      users: [
        { name: "Polok Banik", email: "polok@test.com" },
        { name: "Kopil Banik", email: "kopil@test.com" },
        { name: "Nisha Kuri", email: "nishan@test.com" },
        { name: "Showrov Saha", email: "showrov@test.com" },
      ],
    };
  },
};
</script>

<style scoped>
h1 {
  text-align: center;
}
</style>
