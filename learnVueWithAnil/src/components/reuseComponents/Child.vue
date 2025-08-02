<template>
  <h2>
    {{ data.name }}
    <br />
    {{ data.email }}
  </h2>
  <button @click="getNameData(data.name)">Click here</button>
</template>

<script>
export default {
  name: "Child",

  props: {
    data: Object,
    getNameData: Function,
  },
};
</script>

<style scoped>
h2 {
  background-color: skyblue;
  padding: 10px;
}
</style>
