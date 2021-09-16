<template>
	<main class="mt-5">
		<Jumbo />
		<Courses />
		<Tutoring />
	</main>
</template>

<script>
import Jumbo from "./main-components/Jumbo.vue";
import Courses from "./main-components/courses-components/Courses.vue";
import Tutoring from "./main-components/Tutoring.vue";

export default {
	name: "Main",
	components: {
		Jumbo,
		Courses,
		Tutoring,
	},
};
</script>

<style scoped lang="scss"></style>
