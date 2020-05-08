<template>
	<div class="font-jost min-h-screen tracking-wider leading-normal flex" id="app">
		<Sidebar />
		<Content />
	</div>
</template>

<script>
import Sidebar from './components/Sidebar.vue';
import Content from './components/Content.vue';

export default {
	name: 'App',
	components: {
		Sidebar,
		Content,
	},
};
</script>

<style src="./assets/css/tailwind.css"></style>
