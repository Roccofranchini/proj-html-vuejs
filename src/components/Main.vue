<template>
	<main class="mt-5">
		<Jumbo />
		<Courses />
		<Tutoring />
		<Learners />
		<Blogs />
	</main>
</template>

<script>
import Jumbo from "./main-components/Jumbo.vue";
import Courses from "./main-components/courses-components/Courses.vue";
import Tutoring from "./main-components/Tutoring.vue";
import Learners from "./main-components/learners-components/Learners.vue";
import Blogs from "./main-components/Blogs.vue";

export default {
	name: "Main",
	components: {
		Jumbo,
		Courses,
		Tutoring,
		Learners,
		Blogs,
	},
};
</script>

<style scoped lang="scss"></style>
