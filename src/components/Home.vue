<template>
	<div class="grid gap-y-3">
		<div
			v-for="video in videos.data"
			:key="video.id"
			class="relative w-screen"
			style="padding-top: 56.25%"
		>
			<iframe
				:id="video.id"
				:src="`${video.url}?fs=0&modestbranding=1&playsinline=1&rel=0`"
				allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
				frameborder="0"
				class="absolute top-0 left-0 w-full h-full"
			>
				></iframe
			>
		</div>
	</div>
</template>

<script>
import videos from '../../data/videos.json';

export default {
	data: () => ({
		videos,
	}),
};
</script>

<style scoped>
iframe {
	min-width: 321px;
}
</style>
