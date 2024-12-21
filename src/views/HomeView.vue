<script setup lang="ts">
	import { useSearchStore } from '@/stores/search';

	const searchStore = useSearchStore();
</script>

<template>
  <main>
		<div>teste {{ searchStore.searchQuery }}</div>
	</main>
</template>
