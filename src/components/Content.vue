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

		<!-- Cards Section -->
		<div class="flex flex-wrap w-full mb-6">
			<div class="w-1/2" v-for="(item, index) in array" :key="item.id">
				<!-- Card component -->
				<Card :array="array[index]" />
			</div>
		</div>

		<!-- Border -->
		<div class="border-b border-gray-500 mb-8 mx-2"></div>

		<!-- New Apps and Games Section -->
		<!-- Title - New Apps and Games Section -->
		<div class="flex justify-between mx-2 mb-4">
			<h1 class="font-normal text-lg">New Apps and Games We Love</h1>
			<a class="text-blue-700 hover:text-blue-500" href="#">See all</a>
		</div>

		<!-- AppsGames component -->
		<div class="flex flex-wrap w-full mb-4">
			<div class="w-1/2" v-for="(item, index) in data" :key="item.id">
				<AppsGames :data="data[index]" />
			</div>
		</div>

		<!-- Top Paid Section -->
		<!-- Title - New Apps and Games Section -->
		<div class="flex justify-between mx-2 mb-4">
			<h1 class="font-normal text-lg">Top Paid</h1>
			<a class="text-blue-700 hover:text-blue-500" href="#">See all</a>
		</div>

		<!-- TopPaid component -->
		<div class="flex flex-wrap w-full mb-4">
			<div class="w-1/2" v-for="(item, index) in property" :key="item.id">
				<TopPaid :property="property[index]" />
			</div>
		</div>
	</div>
</template>

<script>
import Card from './Card';
import AppsGames from './AppsGames';
import TopPaid from './TopPaid';

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
			data: [
				{
					title: 'OmniFocus 2',
					subtitle: 'App',
					img: 'icon_omnifocus.png',
					msg: 'Buy',
				},
				{
					title: 'Old Man',
					subtitle: 'Game',
					img: 'icon_daisydisk.png',
					msg: 'Buy',
				},
				{
					title: 'QuarkXPress 2018 Pro',
					subtitle: 'App',
					img: 'icon_quark.png',
					msg: 'Buy',
				},
				{
					title: 'Pixelmator',
					subtitle: 'Game',
					img: 'icon_pixelmator.png',
					msg: 'Buy',
				},
			],
			property: [
				{
					title: '1. Final Cut Pro',
					subtitle: 'Professional post-production',
					img: 'icon_fcp.png',
					price: '40.00$',
				},
				{
					title: '2. Magnet',
					subtitle: 'Organize Your Workspace',
					img: 'icon_magnet.png',
					price: '40.00$',
				},
				{
					title: '3. DaisyDisk',
					subtitle: 'Recover disk space',
					img: 'icon_daisydisk.png',
					price: '40.00$',
				},
				{
					title: '4. The Sims 2: Super Collection',
					subtitle: 'Your faves in one place',
					img: 'icon_sims.png',
					price: '40.00$',
				},
				{
					title: '5. Word Document Writer Pro',
					subtitle: 'Business',
					img: 'icon_word.png',
					price: '40.00$',
				},
				{
					title: '6. Antivirus Zap - Virus & Adware',
					subtitle: 'Scan & Remove Malware & Adware',
					img: 'icon_antivirusapp.png',
					price: '40.00$',
				},
			],
		};
	},
	components: {
		Card,
		AppsGames,
		TopPaid,
	},
};
</script>

<style src="../assets/css/tailwind.css"></style>
