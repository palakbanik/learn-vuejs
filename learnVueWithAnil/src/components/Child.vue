<template>
	<h2>{{ heading }}</h2>
	<h2>{{ name }}</h2>
	<h2>{{ age }}</h2>

	<ul>
		<li v-for="user in usersDetails">Name: {{ user.name }} <br> age: {{
			user.age }}</li>
	</ul>

	<li>{{ getData.name }}</li>

	<button @click="getData()">Click here</button>
</template>

<script>
export default {
	// name: "Child",
	name: "Child",
	data() {
		return {

		}
	},

	props: {
		name: String,
		heading: String,
		age: Number,
		usersDetails: Array,
		getData: Function,
	}


}
</script>

<style></style>