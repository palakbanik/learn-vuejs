<template>

	<h1>Conditional Rendering with (if and else)</h1>

	<div>
		<h2 v-if="showCondition">If Condition</h2>
		<h2 v-else>Else Condition</h2>

		<button @click="changeCondition">Change Condition</button>
	</div>
</template>

<script>
export default {
	data() {
		return {
			showCondition: false,
		}
	},

	methods: {
		changeCondition() {
			this.showCondition = !this.showCondition
		}
	}
}

</script>

<style></style>
