<template>
	<div v-for="video in videos.data" :key="video.id">
		<iframe
			:id="video.id"
			:src="`${video.url}?fs=0&modestbranding=1&playsinline=1&rel=0`"
			allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
			width="640"
			height="360"
			frameborder="0"
		></iframe>
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

<style scoped></style>
