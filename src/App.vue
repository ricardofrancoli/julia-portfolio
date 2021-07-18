<template>
	<div>
		<InfoBar />
		<Home />
	</div>
</template>

<script>
import InfoBar from './components/InfoBar.vue';
import Home from './components/Home.vue';

export default {
	components: {
		InfoBar,
		Home,
	},
};
</script>

<style scoped></style>
