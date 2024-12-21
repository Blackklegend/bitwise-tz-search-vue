<script setup lang="ts">
import PageHeader from './components/PageHeader.vue';
import { RouterLink, RouterView } from 'vue-router';

</script>

<template>
	<div class="bg-slate-50 min-h-screen">
		<PageHeader />
		<RouterView />
	</div>
</template>

<style scoped>

</style>
