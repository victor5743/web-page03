<template>
	<div class="w-1/2 bg-dark flex px-8 py-6 items-center">
		<div class="flex-1">
			<div class="uppercase mb-4">{{ array.subtitle }}</div>
			<h1 class="font-normal text-2xl mb-4">{{ array.title }}</h1>
			<p class="text-gray-400 text-xs leading-normal">{{ array.content }}</p>
		</div>
		<div class="w-1/3">
			<img class="rounded-full" :src="require(`@/assets/${array.url}`)" alt="cover" />
		</div>
	</div>
</template>

<script>
export default {
	props: ['array'],
};
</script>
