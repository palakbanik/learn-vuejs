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
	<!-- <ConditionalRendering /> -->
	<!-- <ConditionalRendering /> -->
	<!-- <ForLoopAndList /> -->
	<!-- <Child heading="Child Components" name="Polok Banik" :age=23 :usersDetails="users" :getData="getData" /> -->
	<Parent />
</template>

<script>
import CheckBoxAndRadioValue from "./components/CheckBoxAndRadioValue.vue";
import ConditionalRendering from "./components/ConditionalRendering.vue";
import TwoWayBinding from "./components/twoWayBinding.vue";
import VModel from "./components/VModel.vue";
import ForLoopAndList from "./components/ForLoopAndList.vue";
import Child from "./components/Child.vue";
import Parent from "./components/reuseComponents/Parent.vue";
export default {
	components: {
		VModel,
		TwoWayBinding,
		CheckBoxAndRadioValue,
		ConditionalRendering,
		ForLoopAndList,
		Child,
		Parent
	},

	data() {
		return {
			users: [
				{ name: "Polok", age: 23 },
				{ name: "Nishan", age: 24 },
				{ name: "Kopil", age: 25 },
				{ name: "Showrov", age: 26 },
			]
		}
	},

	methods: {
		getData() {
			alert("function is called")
		}
	}

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
