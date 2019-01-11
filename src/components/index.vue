<template>
	<div>
		<headerContainer />
		<tabsContainer />
	</div>
</template>

<script>
	import headerContainer from './header/index.vue';
	import tabsContainer from './tabs/tabs.vue';
	export default {
		name: 'index',
		components: {
			headerContainer: headerContainer,
			tabsContainer: tabsContainer,
		},
		data() {
			return {

			};
		},
	}
</script>

<style>

</style>
