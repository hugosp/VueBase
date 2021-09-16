<template>
	<Navbar title="Template" :links="links" />
	<router-view />
</template>

<script>
import Navbar from './components/Navbar.vue';
export default {
	data() {
		return {
			links: [
				{ id: 1, name: 'Home', path: '/' },
				{ id: 2, name: 'About', path: '/about' },
				{ id: 3, name: 'Contact', path: '/contact' },
			],
		};
	},
	components: {
		Navbar,
	},
};
</script>


<style lang="scss">
@import url('https://cdn.jsdelivr.net/npm/water.css@2/out/water.min.css');
body {
	max-width: 90vw;
}
</style>
