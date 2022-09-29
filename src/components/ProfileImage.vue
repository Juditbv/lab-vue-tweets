<script setup>
	const props = defineProps({
		image: String,
	});
</script>

<template>
	<img
		referrerpolicy="no-referrer"
		:src="image"
		class="profile"
		alt="profile"
	/>
</template>


<style scoped>
</style>