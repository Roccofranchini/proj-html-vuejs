<template>
	<!-- SINGLE STAT STRUCTURE -->
	<div class="col-3 border-start border-end">
		<div class="d-flex flex-column text-center py-2">
			<h6 class="my-blue px-5 mt-5">{{ stat.title }}</h6>
			<h2 class="my-primary pt-3 pb-2">{{ stat.number }}</h2>
			<p class="my-gray mb-5">{{ stat.subtitle }}</p>
		</div>
	</div>
</template>

<script>
export default {
	name: "Stat",
	props: ["stat"],
};
</script>

<style scoped lang="scss">
//SCSS

.col-3 {
	h6 {
		font-weight: 700;
		font-size: 17px;
	}
	h2 {
		font-family: "Roboto", sans-serif;
		font-weight: 900;
		font-size: 50px;
	}
	p {
		font-size: 13px;
		font-weight: 700;
		letter-spacing: 2px;
	}
}
</style>
