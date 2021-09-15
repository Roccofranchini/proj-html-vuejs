<template>
	<main class="mt-5">
		<Jumbo />
		<Courses />
	</main>
</template>

<script>
import Jumbo from "./main-components/Jumbo.vue";
import Courses from "./main-components/courses-components/Courses.vue";

export default {
	name: "Main",
	components: {
		Jumbo,
		Courses,
	},
};
</script>

<style scoped lang="scss"></style>
