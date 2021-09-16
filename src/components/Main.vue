<template>
	<main class="mt-5">
		<Jumbo />
		<Courses />
		<Tutoring />
		<Learners />
	</main>
</template>

<script>
import Jumbo from "./main-components/Jumbo.vue";
import Courses from "./main-components/courses-components/Courses.vue";
import Tutoring from "./main-components/Tutoring.vue";
import Learners from "./main-components/learners-components/Learners.vue";

export default {
	name: "Main",
	components: {
		Jumbo,
		Courses,
		Tutoring,
		Learners,
	},
};
</script>

<style scoped lang="scss"></style>
