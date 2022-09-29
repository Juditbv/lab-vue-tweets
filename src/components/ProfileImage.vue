<script setup>
	const props = defineProps({
		image: String,
	});
</script>

<template>
	<img
		referrerpolicy="no-referrer"
		:src="props.tweet.user.image"
		class="profile"
		alt="profile"
	/>
</template>


<style lang="scss" scoped>
</style>