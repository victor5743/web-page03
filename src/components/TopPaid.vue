<template>
	<div
		class="flex justify-between items-center h-full mx-2 border-b boder-gray-600 mb-2 py-2"
	>
		<img class="h-24" :src="require(`@/assets/${property.img}`)" alt="Icon" />
		<div class="px-6 mt-2">
			<p class="font-semibold">{{ property.title }}</p>
			<p class="mb-1 text-xs">{{ property.subtitle }}</p>
		</div>
		<div>
			<a
				href="#"
				class="bg-white text-blue-500 rounded-full my-2 px-6 py-1 text-xs font-bold text-center w-24 hover:bg-light hover:text-white"
			>
				BUY
			</a>
		</div>
	</div>
</template>

<script>
export default {
	props: ['property'],
};
</script>
