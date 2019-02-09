<template>
	<section id="profile">
		<img v-bind:src="user.image" alt="" />
		<h3>{{ user.name }}</h3>
	</section>
</template>

<script>
	export default {
		name: "Profile",
		props: {
			user: Object
		}
	}
</script>

<style scoped>
	#profile {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 15px;
	}

	#profile img {
		width: 50%;
	}
</style>


