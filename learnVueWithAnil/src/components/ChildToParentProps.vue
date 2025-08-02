<template>
  <h1>Child to Parent pass a data.</h1>

  <button @click="passData(fullName)">show alert</button>
</template>

<script>
export default {
  name: "ChildToParentProps",
  data() {
    return {
      fullName: "Polok Banik", // I am sending this value to the parent component.
    };
  },

  props: {
    passData: Function,
  },
};
</script>

<style></style>
