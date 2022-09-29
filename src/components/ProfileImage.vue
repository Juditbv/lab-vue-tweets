<script setup>
	const props = defineProps({
		imageDog: String,
	});
</script>

<template>
	<img
		:src="props.imageDog"
		class="profile"
		alt="profile"
		referrerpolicy="no-referrer"
	/>
</template>