<script setup lang="ts">
import { useSearchStore } from "@/stores/search";

const searchStore = useSearchStore();

const handleSearch = () => {
	alert(searchStore.searchQuery);
};
</script>
<template>
	<header class="p-4 flex flex-col sm:flex-row shadow">
		<span class="flex-auto basis-4/6 text-center sm:text-left mb-3 sm:mb-0 font-bold align-middle h-full">Bitwise
			timezone search</span>
		<div class="basis-2/6 place-items-center sm:place-items-end flex-auto">
			<div class="flex flex-nowrap">
				<input type="text" class="rounded-lg px-2 py-1 rounded-r-none" placeholder="Type the timezone offset"
					v-model="searchStore.searchQuery" />
				<button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-1 px-2 rounded rounded-l-none"
					@click="handleSearch">
					Search
				</button>
			</div>
		</div>
	</header>
</template>

<style lang="css"></style>
