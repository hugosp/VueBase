<template>
	<nav>
		<div class="title">
			{{ title }}
		</div>

		<div class="links">
			<div v-for="link in links" :key="link.id">
				<router-link :to="link.path">
					{{ link.name }}
				</router-link>
			</div>
		</div>

		<button>Login</button>
	</nav>
</template>

<script>
export default {
	props: {
		title: { type: String, required: true },
		links: { type: Array, required: true },
	},
};
</script>

<style lang="scss" scoped>
nav {
	display: grid;
	grid-template-columns: 1fr 1fr 1fr;

	.title {
		font-size: 30px;
		font-weight: bold;
	}

	.links {
		display: grid;
		grid-template-columns: repeat(3, 1fr);
		div {
			margin: auto;
		}
	}
	button {
		width: 50%;
		margin: auto 0 auto auto;
	}
}
</style>
