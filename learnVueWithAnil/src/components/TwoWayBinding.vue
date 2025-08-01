<template>
	<form action="/login" method="POST">
		<input type="text" name="username" placeholder="enter email" v-model="showEmail" />
		<br />
		<br />
		<input type="password" name="username" placeholder="enter password" v-model="showPass" />
		<br />
		<br />

		<button @click="getValues" type="button">Login</button>
	</form>
</template>

<script>
export default {
	name: "TwoWayBinding",

	data() {
		return {
			showEmail: null,
			showPass: null,
		};
	},

	methods: {
		getValues() {
			console.log("email: ", this.showEmail);
			console.log("password: ", this.showPass);
		},
	},
};
</script>

<style></style>
