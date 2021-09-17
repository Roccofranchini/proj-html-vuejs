<template>
	<div id="learners" class="pt-5">
		<!-- LEARNERS  STRUCTURE -->
		<div class="text-center pb-4">
			<!-- TITLE -->
			<p class="my-gray subtitle mb-2">
				GREAT WORDS ABOUT MAXCOACH
			</p>
			<h3 class="my-blue title">
				Our <span class="my-primary">top learners'</span> verbatim
			</h3>
		</div>
		<div class="fake-container mx-5">
			<!-- STUDENTS -->
			<div class="row g-5">
				<Student
					v-for="(student, index) in students"
					:key="index"
					:student="student"
					:index="index"
					@change="change"
				/>
			</div>
		</div>
		<div class="container my-5">
			<!-- GET STARTED -->

			<div class="row">
				<div class="col-2 d-flex flex-column justify-content-center">
					<div class="circle ms-4"></div>
					<img
						class="pt-3 ms-4 w-75"
						src="./../../../assets/img/maxcoach-shape-01.png"
						alt=""
					/>
				</div>
				<div class="col-8">
					<div
						class="certification-text d-flex flex-column align-items-center mt-5"
					>
						<p class="my-blue mb-1">
							Start today for getting<span class="my-primary">
								Online Certification</span
							>
						</p>
						<h4 class="my-blue pb-4">
							You can be your own guidinig star whit our help!
						</h4>
						<button class="button-primary px-5">Get started now</button>
					</div>
				</div>
				<div class="col-2 d-flex align-items-end">
					<img
						class="h-75 pt-5"
						src="./../../../assets/img/maxcoach-shape-02.png"
						alt=""
					/>
				</div>
			</div>
		</div>
		<!-- STATISTICS -->

		<Stats />
	</div>
</template>

<script>
//IMPORT VARS

import Student from "./Student.vue";
import Stats from "./Stats.vue";

export default {
	name: "Learners",
	components: {
		Student,
		Stats,
	},
	methods: {
		// CHANGE THE ACTIVE CARD [tofix]

		change(index) {
			console.log(index);

			if (index == 0) {
				if (
					!this.students[0].visible &&
					!this.students[1].visible &&
					this.students[2].visible
				) {
					this.students[0].visible = true;
					this.students[1].visible = false;
					this.students[2].visible = false;
				}
				if (
					!this.students[0].visible &&
					this.students[1].visible &&
					!this.students[2].visible
				) {
					this.students[0].visible = true;
					this.students[1].visible = false;
					this.students[2].visible = false;
				}
				if (
					this.students[0].visible &&
					!this.students[1].visible &&
					!this.students[2].visible
				) {
					this.students[0].visible = true;
					this.students[1].visible = false;
					this.students[2].visible = false;
				}
			}
			if (index == 1) {
				if (
					!this.students[0].visible &&
					!this.students[1].visible &&
					this.students[2].visible
				) {
					this.students[0].visible = false;
					this.students[1].visible = true;
					this.students[2].visible = false;
				}
				if (
					!this.students[0].visible &&
					this.students[1].visible &&
					!this.students[2].visible
				) {
					this.students[0].visible = false;
					this.students[1].visible = true;
					this.students[2].visible = false;
				}
				if (
					this.students[0].visible &&
					!this.students[1].visible &&
					!this.students[2].visible
				) {
					this.students[0].visible = false;
					this.students[1].visible = true;
					this.students[2].visible = false;
				}
			}
			if (index == 2) {
				if (
					!this.students[0].visible &&
					!this.students[1].visible &&
					this.students[2].visible
				) {
					this.students[0].visible = false;
					this.students[1].visible = false;
					this.students[2].visible = true;
				}
				if (
					!this.students[0].visible &&
					this.students[1].visible &&
					!this.students[2].visible
				) {
					this.students[0].visible = false;
					this.students[1].visible = false;
					this.students[2].visible = true;
				}
				if (
					this.students[0].visible &&
					!this.students[1].visible &&
					!this.students[2].visible
				) {
					this.students[0].visible = false;
					this.students[1].visible = false;
					this.students[2].visible = true;
				}
			}
		},
	},
	data() {
		return {
			students: [
				{
					name: "FLORENCE  THEMES",
					visible: false,
					profession: "Multimedia Admin",
					img: "testimonial-avata-03",
					title: "It's a choiche for people with a special needs",
					text:
						"I'm a very strict person so i require everything to be organized and neat. then, i'll be able to makw thingd right and shine. MaxCoach guys just got me. ",
				},
				{
					name: "MINA  HOLLACE",
					visible: true,
					profession: "Freelancer",
					img: "testimonial-avata-02",
					title: "High levels of inefficiency and scientific teaching methods",
					text:
						"I am free to learn at my own pace, follow my own schedule and choose the subject i want to learn from the syllabus. Great study portal for people like me.",
				},
				{
					name: "FLORENCE  THEMES",
					visible: false,
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
};
</script>

<style scoped lang="scss">
//SCSS

#learners {
	background-color: #f8f8f8;

	.circle {
		width: 40px;
		height: 40px;
		border-color: #e6dcd2;
	}

	.certification-text {
		p {
			font-weight: 600;
			font-size: 18px;
		}
		span {
			font-weight: 500;
		}

		h4 {
			font-weight: 700;
		}
	}
}
</style>
