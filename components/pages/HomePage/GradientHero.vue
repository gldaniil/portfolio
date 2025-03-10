<template>
	<div class="absolute h-full w-full flex justify-center items-center -z-10">
		<div
			class="bg-gradient-to-r from-sky-600 from-14% to-purple-700 blur-[75px] opacity-60 animate-rotate"
		/>
	</div>
</template>

<script setup></script>
<style scoped>
@keyframes rotate {
	0% {
		transform: rotate(0deg);
	}
	100% {
		transform: rotate(360deg);
	}
}
@keyframes resize {
	0% {
		width: 45vw;
		height: 30vw;
	}
	100% {
		width: 30vw;
		height: 45vw;
	}
}
@keyframes round {
	0% {
		border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%;
	}
	25% {
		border-radius: 35% 65% 65% 35% / 35% 35% 65% 65%;
	}
	50% {
		border-radius: 40% 60% 60% 40% / 40% 40% 60% 60%;
	}
	75% {
		border-radius: 35% 65% 65% 35% / 35% 35% 65% 65%;
	}
	100% {
		border-radius: 45% 85% 85% 45% / 45% 45% 85% 85%;
	}
}
.animate-rotate {
	animation: rotate 40s cubic-bezier(0.8, 0.2, 0.2, 0.8) alternate infinite,
		round 7s linear alternate infinite, resize 12s linear alternate infinite;
}
</style>
