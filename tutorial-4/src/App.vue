<template>
  <!-- <div>{{ books }}</div>
  <h1>{{ isBookEvenOrOdd() }}</h1>
  <h1>{{ isBookEvenOrOdd() }}</h1>
  <h1>{{ isBookEvenOrOdd() }}</h1>

  <h2>{{ computedIsEvenOrOdd }}</h2>
  <h2>{{ computedIsEvenOrOdd }}</h2>
  <h2>{{ computedIsEvenOrOdd }}</h2>

  <button @click="pushBtn">add more book</button>
  <button @click="counter++">Count {{ counter }}</button> -->

  <!-- <p>has published books:</p>
  <span>{{ author.books.length > 0 ? "yes" : "no" }}</span> -->

  <div :class="classObject">Hello world</div>
</template>

<script>
export default {
  //   data() {
  //     return {
  //       counter: 0,
  //       books: [
  //         { id: 1, bookName: "Atomic" },
  //         { id: 2, bookName: "Atomic" },
  //         { id: 3, bookName: "Atomic" },
  //         { id: 4, bookName: "Atomic" },
  //       ],
  //     };
  //   },
  //   data() {
  //     return {
  //       author: {
  //         name: "John Doe",
  //         books: [
  //           "Vue 2 - Advanced Guide",
  //           "Vue 3 - Basic Guide",
  //           "Vue 4 - The Mystery",
  //         ],
  //       },
  //     };
  //   },
  //   methods: {
  //     isBookEvenOrOdd() {
  //       console.log("check");
  //       return this.books.length % 2 === 0 ? "EVEN" : "ODD";
  //     },
  //     pushBtn() {
  //       this.computedIsEvenOrOdd = "EVEN";
  //       this.books.push({
  //         id: 5,
  //         name: "Polok",
  //       });
  //     },
  //   },
  //   computed: {
  //     computedIsEvenOrOdd() {
  //       console.log("computed checked");
  //       return this.books.length % 2 === 0 ? "EVEN" : "ODD";
  //     },
  //   },

  data() {
    return {
      //   isActive: true,
      //   error: null,

      isActive: true,
      error: null,
    };
  },

  computed: {
    classObject() {
      return {
        active: this.isActive && !this.error,

        "text-danger": this.error && this.error.type === "fatal",
        // active: this.isActive && !this.error,
        // "text-danger": this.error && this.error.type === "fatal",
      };
    },
  },
};
</script>

<style>
.text-danger {
  color: red;
}

.active {
  color: green;
}
</style>
