<template>
	<section id="stats">
		<!-- STATS STRUCTURE -->

		<div class="container">
			<div class="row">
				<!-- SINGLE STAT V-FOR -->
				<Stat v-for="(stat, index) in stats" :key="index" :stat="stat" />
			</div>
		</div>
	</section>
</template>

<script>
//IMPORT COMPONENTS

import Stat from "./Stat.vue";

export default {
	name: "Stats",
	components: {
		Stat,
	},
	data() {
		return {
			stats: [
				{
					title: "Succesfully trained",
					number: 1790,
					subtitle: "ENROLLED LEARNERS",
				},
				{
					title: "Proudly Received",
					number: 19,
					subtitle: "COUNTRYWIDE AWARDS",
				},
				{
					title: "Firmly Estabilished",
					number: 24,
					subtitle: "LOCAL BRANCHES",
				},
				{
					title: "Getting Featured on",
					number: 1090,
					subtitle: "BLOG POSTS",
				},
			],
		};
	},
};
</script>

<style scoped lang="scss">
//SCSS

#stats {
	background-color: white;
}
</style>
