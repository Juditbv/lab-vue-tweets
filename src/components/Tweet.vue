<script setup>
	import ProfileImage from "./ProfileImage.vue";
	import User from "./User.vue";
	import Timestamp from "./Timestamp.vue";
	import Message from "./Message.vue";
	import Actions from "./Actions.vue";
	const props = defineProps({
		message: String,
		timestamp: String,
		user: Object,
		image: String,
	});
</script>

<template>
	<div class="tweet">
		<ProfileImage :imageDog="props.image" />

		<div class="body">
			<div class="top">
				<User :user-data="props.user" />

				<Timestamp :time="props.timestamp" />
			</div>

			<Message :message="props.message" />

			<Actions />
		</div>
	</div>
</template>

<style scoped>
	a {
		color: #42b983;
	}
</style>