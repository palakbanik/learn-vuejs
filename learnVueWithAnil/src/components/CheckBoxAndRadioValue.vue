<template>
	<h1>Get Checkbox & Radio Button Value</h1>

	<div>

		<h2>Technology</h2>
		<input type="checkbox" value="java" id="java" v-model="technology">
		<label for="java">Java</label>
		<input type="checkbox" value="php" id="php" v-model="technology">
		<label for="php">Php</label>
		<input type="checkbox" value="node" id="node" v-model="technology">
		<label for="node">Node</label>

		<h4>Language: {{ technology }}</h4>
	</div>
</template>

<script>
export default {
	name: "CheckBoxAndRadioValue",

	data() {
		return {
			technology: []
		}
	}
};
</script>

<style></style>
