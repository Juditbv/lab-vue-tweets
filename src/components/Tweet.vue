<script setup>
	import ProfileImage from "./ProfileImage.vue";
	import User from "./User.vue";
	import Timestamp from "./Timestamp.vue";
	import Message from "./Message.vue";
	import Actions from "./Actions.vue";
	const props = defineProps({
		tweetContent: Object,
	});
</script>

<template>
	<div class="tweet">
		<ProfileImage :image="props.tweetContent.user.image" />

		<div class="body">
			<div class="top">
				<User :user-data="props.tweetContent.user" />

				<Timestamp :time="props.tweetContent.timestamp" />
			</div>

			<Message :message="props.tweetContent.message" />

			<Actions />
		</div>
	</div>
</template>

<style scoped>
	a {
		color: #42b983;
	}
</style>