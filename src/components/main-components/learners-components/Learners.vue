<template>
	<div id="learners" class="py-5">
		<div class="text-center pb-4">
			<p class="my-gray learners-subtitle mb-2">
				GREAT WORDS ABOUT MAXCOACH
			</p>
			<h3 class="my-blue learners-title">
				Our <span class="my-primary">top learners'</span> verbatim
			</h3>
		</div>
		<div class="fake-container mx-5">
			<div class="row g-5">
				<Student
					v-for="(student, index) in students"
					:key="index"
					:student="student"
				/>
			</div>
		</div>
	</div>
</template>

<script>
import Student from "./Student.vue";

export default {
	name: "Learners",
	data() {
		return {
			students: [
				{
					name: "FLORENCE  THEMES",
					profession: "Multimedia Admin",
					img: "testimonial-avata-03",
					title: "it's a choiche for people with a special needs",
					text:
						"I'm a very strict person so i require everything to be organized and neat. then, i'll be able to makw thingd right and shine. MaxCoach guys just got me. ",
				},
				{
					name: "MINA  HOLLACE",
					profession: "Freelancer",
					img: "testimonial-avata-02",
					title: "High levels of inefficiency and scientific teaching methods",
					text:
						"I am free to learn at my own pace, follow my own schedule and choose the subject i want to learn from the syllabus. Great study portal for people like me.",
				},
				{
					name: "FLORENCE  THEMES",
					profession: "IT Specialist",
					img: "testimonial-avata-04",
					title:
						"Prpfessional team of specialists and passionate mentors at reach",
					text:
						"I need to get a certification for English proficiency and MaxCoach is my best choice. Their tuthors are smart and professional when dealing with students.",
				},
			],
		};
	},
	components: {
		Student,
	},
};
</script>

<style scoped lang="scss">
#learners {
	background-color: #f5f7fa;

	.learners-subtitle {
		font-size: 11px;
		font-weight: 500;
		letter-spacing: 2px;
	}
	.learners-title {
		font-weight: 700;

		span {
			font-weight: 500;
		}
	}
}
</style>
