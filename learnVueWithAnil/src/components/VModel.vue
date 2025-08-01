<template>
	<input type="text" v-model="count" />
	<!-- // v-model er kaaj holo input box er
  vitor jei value ta user dibe seta ta sathe sathe get kore fela... -->

	<h2>{{ count }}</h2>
</template>

<script>
export default {
	name: 'v-model',

	data() {
		return {
			count: "",
		};
	},
};
</script>

<style></style>
