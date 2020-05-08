<template>
	<div class="font-jost min-h-screen tracking-wider leading-normal" id="app">
		<HelloWorld />
	</div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
	name: 'App',
	components: {
		HelloWorld,
	},
};
</script>

<style src="./assets/css/tailwind.css"></style>
