<template>
	<!-- <h1 v-if="headingHide === true">Home Component</h1>

  <button v-on:click="showHeading">click here</button>
  <button v-on:dblclick="getData('Button double clicked')">click here</button>
  <br />
  <br />
  <button @click="counter">counter {{ count }}</button> -->

	<!-- <h1>Email is: {{ email }}</h1>
  <h1>Number is: {{ number }}</h1>
  <h1>Name is: {{ name }}</h1> -->

	<!-- <VModel />	 -->
	<!-- <TwoWayBinding /> -->
	<!-- <ChechBoxAndRadionValue /> -->
	<ConditionalRendering />
</template>

<script>
import ChechBoxAndRadionValue from "./components/ChechBoxAndRadionValue.vue";
import ConditionalRendering from "./components/ConditionalRendering.vue";
import TwoWayBinding from "./components/twoWayBinding.vue";
import VModel from "./components/v-model.vue";
export default {
	components: {
		VModel,
		TwoWayBinding,
		ChechBoxAndRadionValue,
		ConditionalRendering,
	},

	//   data() {
	//     return {
	//       //   name: "Polok Banik",
	//       //   email: "abc@gmail.com",
	//       //   number: 12345,
	//       headingHide: false,
	//       count: 0,
	//     };
	//   },
	//   methods: {
	//     getData(getValue) {
	//       alert(getValue);
	//     },
	//     getConsole() {
	//       console.warn("mouse down the heading");
	//     },
	//     showHeading() {
	//       this.headingHide = !this.headingHide;
	//     },
	//     counter() {
	//       this.count++;
	//     },
	//   },
};
</script>

<style scoped></style>
