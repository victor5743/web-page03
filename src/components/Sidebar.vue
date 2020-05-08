<template>
	<div class="bg-dark w-1/4 pt-8 text-white border-r-2 border-darkest">
		<!-- Input and SVG -->
		<div class="text-center p-4 relative flex">
			<!-- Input -->
			<input
				class="rounded-sm p-2 pl-8 w-full text-white bg-light border border-gray-500 outline-none focus:border-gray-300"
				type="text"
				placeholder="Search"
			/>

			<!-- SVG -->
			<div class="absolute py-3 px-2 text-gray-500">
				<svg
					class="fill-current"
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 20 20"
					width="18"
					height="18"
				>
					<path
						d="M12.9 14.32a8 8 0 1 1 1.41-1.41l5.35 5.33-1.42 1.42-5.33-5.34zM8 14A6 6 0 1 0 8 2a6 6 0 0 0 0 12z"
					/>
				</svg>
			</div>
		</div>
	</div>
</template>

<script>
export default {};
</script>
