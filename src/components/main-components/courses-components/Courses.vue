<template>
	<section id="courses">
		<div class="container">
			<div class="text-center mb-5 pb-4">
				<p class="my-gray courses-subtitle">STIMULATED TO LEARN?</p>
				<h3 class="my-blue courses-title">Featured Online Courses</h3>
			</div>
			<div class="row gy-5">
				<Card
					v-for="(course, index) in courses"
					:key="index"
					:course="course"
				/>
			</div>
			<div class="row justify-content-center">
				<div class="col-8 text-center">
					<button class="button-primary mt-5">
						View all courses <i class="fas fa-arrow-right"></i>
					</button>
				</div>
			</div>
		</div>
	</section>
</template>

<script>
import Card from "./Card.vue";

export default {
	name: "Courses",
	components: {
		Card,
	},
	data() {
		return {
			courses: [
				{
					img: "course-02-480x298",
					title: "Learning to Write as a Professional Author",
					lessons: 20,
					students: 50,
					price: "40.00",
				},
				{
					img: "stock-full-hd-03-480x298",
					title: "Customer-centric Info-Tech Strategies",
					lessons: 24,
					students: 769,
					price: "Free",
				},
				{
					img: "stock-full-hd-04-480x298",
					title: "Open Programming Courses for Everyone: Python",
					lessons: 17,
					students: 62,
					price: "19.00",
				},
				{
					img: "stock-full-hd-06-480x298",
					title: "Academic Listening and Note-taking",
					lessons: 14,
					students: 67,
					price: "26.00",
				},
				{
					img: "course-featured-image-01-480x298",
					title: "Master jQuery in a Short Period of Time",
					lessons: 6,
					students: 51,
					price: "39.00",
				},
				{
					img: "stock-full-hd-05-480x298",
					title: "Introduction to javascript for Beginners",
					lessons: 14,
					students: 76,
					price: "59.00",
				},
			],
		};
	},
};
</script>

<style scoped lang="scss">
@import "@/assets/scss/_variables.scss";

#courses {
	padding: 100px 0;

	background-color: #f5f7fa;

	.courses-subtitle {
		font-size: 11px;
		font-weight: 500;
		letter-spacing: 2px;
	}
	.courses-title {
		font-weight: 700;
	}

	button {
		padding: 13px 70px;
	}
}
</style>
