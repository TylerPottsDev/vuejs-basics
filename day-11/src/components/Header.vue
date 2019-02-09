<template>
	<header>
		<div class="logo">
			<img src="../assets/logo.png" alt="VueJS Logo" />
		</div>
		<div class="title">
			<h1>{{ title }}</h1>
		</div>
		<div class="filler"></div>
	</header>
</template>

<script>
	export default {
		name: "Header",
		props: {
			title: String
		}
	}
</script>

<style scoped>
	header {
		width: 100%;
		height: 60px;
		background: #171717;

		display: flex;
		justify-content: center;
		align-items: center;
	}

	.logo {
		flex: 1;
	}
	.logo img {
		height: 30px;
	}

	.title {
		flex: 3;
	}

	.title h1 {
		color: #F3F3F3;
		font-size: 28px;
		line-height: 60px;
		font-weight: 300;
	}

	.filler {
		flex: 1;
	}
</style>

