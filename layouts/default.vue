<script setup>
import AppFooter from '~/components/layout/AppFooter.vue';
import AppHeader from '~/components/layout/AppHeader.vue';
</script>

<template>
	<div>
		<AppHeader />
		<main>
			<slot />
		</main>
		<AppFooter />
	</div>
</template>

<style></style>
