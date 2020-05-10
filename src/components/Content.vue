<template>
	<div class="bg-darker w-3/4 text-white px-10">
		<!-- Image and text -->
		<div
			class="discover-banner text-white px-8 rounded-b-lg py-12 bg-no-repeat bg-cover mb-6"
		>
			<span class="uppercase mb-4">The Basics</span>
			<h1 class="font-normal mb-4">Create Personal Projects</h1>
			<p class="w-64 leading-normal text-gray-400">
				With these apps, creativity has no boundaries.
			</p>
		</div>

		<!-- Cards -->
		<div class="flex">
			<div class="w-1/2" v-for="(item, index) in array" :key="item.id">
				<Card :array="array[index]" />
			</div>
		</div>
	</div>
</template>

<script>
import Card from './Card';

export default {
	data() {
		return {
			array: [
				{
					title: 'Edit Photos Fast with Extensions',
					subtitle: 'Get Started',
					content: 'Tweak photos using multiple apps, without switching windows.',
					url: 'discover2.jpg',
				},
				{
					title: '3 Notable Note-Tacking Apps',
					subtitle: 'The basics',
					content: 'Plain text enthusiast? Markdown master? Find your new favourite.',
					url: 'discover3.jpg',
				},
			],
		};
	},
	components: {
		Card,
	},
};
</script>

<style src="../assets/css/tailwind.css"></style>
