<script setup>
	const props = defineProps({
		image: String,
	});
</script>

<template>
	<img
		referrerpolicy="no-referrer"
		:src="props.image"
		class="profile"
		alt="profile"
	/>
</template>