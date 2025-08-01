<template>
	<h1>For Loop in Vue js</h1>

	<ul>
		<li v-for="item in items" key="item">{{ item }}</li>
	</ul>

	<br><br>

	<ul>
		<li v-for="user in users" key="user.index">User name is: {{ user.name }} <br> User email is: {{ user.email }}
		</li>
	</ul>
</template>

<script>
export default {
	name: "ForLoopAndList",

	data() {
		return {
			items: ['java', 'php', 'node', 'html', 'css'],
			users: [
				{ name: "Polok", email: "polok@test.com", index: 1 },
				{ name: "Amit", email: "amit@test.com", index: 2 },
				{ name: "uthpal", email: "utpal@test.com", index: 3 },
				{ name: "Monika", email: "monika@test.com", index: 4 },
			]
		}
	}
}
</script>

<style></style>