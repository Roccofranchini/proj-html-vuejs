<template>
	<div class="background pb-5">
		<section id="tutoring" class="py-5">
			<!-- TUTORING STRUCTURE -->

			<div class="container">
				<!-- TITLE -->
				<div class="text-center my-5 pb-4">
					<p class="my-gray tutoring-subtitle mb-2">
						MAXCOACH AVAILABLE COURSES
					</p>
					<h3 class="my-blue tutoring-title">
						Acces <span class="my-primary">Smart Tutoring</span> Program for
						Benefits.
					</h3>
				</div>
				<!-- PROGRAM v-for -->

				<div class="row my-5 pb-5 gx-5">
					<div
						v-for="(program, index) in programs"
						:key="index"
						class="col tutor-card"
					>
						<img :src="require(`../../assets/img/${program.img}.png`)" alt="" />
						<h4 class="my-blue mt-4 mb-2">{{ program.title }}</h4>
						<p class="my-gray">
							{{ program.text }}
						</p>
						<span class="my-second-blue"
							><a href="">{{ program.link }}</a>
							<i class="fas fa-long-arrow-alt-right"></i
						></span>
					</div>
				</div>
				<div class="row mb-5">
					<div class="col-7 d-flex justify-content-end">
						<!-- TUTORING IMAGES -->

						<div class="images">
							<div class="circle"></div>
							<img
								class="img-fluid img-1"
								src="../../assets/img/home-2-popup-video-poster.jpg"
								alt=""
							/>
							<img
								class="img-2"
								src="../../assets/img/icon-youtube-play.png"
								alt=""
							/>
							<img
								class="img-3"
								src="../../assets/img/maxcoach-shape-05-150x150.png"
								alt=""
							/>
							<img
								class="img-4"
								src="../../assets/img/maxcoach-shape-07-150x150.png"
								alt=""
							/>
						</div>
					</div>
					<div class="col-5">
						<!-- TUTORING TEXT -->

						<div class="text ms-4 pt-4 mt-2">
							<span class="subtitle my-gray"
								>GET STARTED <span class="my-blue">EFFORTLESSLY</span></span
							>
							<h4 class="title my-blue mt-3 mb-0">
								Enjoy Our
							</h4>
							<h4 class="title-primary my-primary mb-4">
								Companionship
							</h4>
							<p class="my-gray pe-5 me-2">
								Sneek peek into ehat has in store for you on our online teaching
								and mentoring portal. Seek for dome hidden hints of early-bird
								rewards as well.
							</p>
							<span class="my-primary"
								>Download free guidebook
								<i class="fas fa-long-arrow-alt-right"></i>
								<hr class="my-gray"
							/></span>
						</div>
					</div>
				</div>
			</div>
		</section>
	</div>
</template>

<script>
export default {
	name: "Tutoring",
	data() {
		return {
			programs: [
				{
					img: "home-2-image-box-01",
					title: "Customize Preferences",
					text:
						"Learners are given the rights to arrange and customize their study schedule and timetable based on preferences",
					link: "Start here ",
				},
				{
					img: "about-us-02-image-box-02",
					title: "Cloud Storage",
					text:
						"You can store online lessons via online cloud or download to yourdevice and revise lessons on the way.",
					link: "Get Free Quote ",
				},
				{
					img: "home-2-image-box-03",
					title: "Multimedia Channels",
					text:
						"We provide study materials with various formats: video, audio,slides. doc, prints, books and applications.",
					link: "Start now ",
				},
			],
		};
	},
};
</script>

<style scoped lang="scss">
//VARS

@import "@/assets/scss/_variables.scss";

//SCSS

.background {
	background-color: #f8f8f8;
}

#tutoring {
	background-color: white;
	border-bottom-right-radius: 50% 20%;
}

.row {
	.tutoring-subtitle {
		font-size: 11px;
		font-weight: 500;
		letter-spacing: 2px;
	}
	.tutoring-title {
		font-weight: 700;

		span {
			font-weight: 500;
		}
	}

	.tutor-card {
		h4 {
			font-size: 20px;
			font-weight: 600;
		}
		p {
			font-size: 12px;
			font-weight: 600;
		}
		span {
			font-weight: 700;
			font-size: 12px;
			a {
				text-decoration: none;
				color: $my-second-blue;
			}
		}
	}
}

.row {
	.images {
		position: relative;
		.img-1 {
			max-height: 330px;
			position: relative;
			z-index: 1;
		}
		.img-2 {
			position: absolute;
			top: 50%;
			right: 50%;
			transform: translate(50%, -50%);
			height: 50px;
			z-index: 2;
		}
		.img-3 {
			position: absolute;
			top: 40px;
			left: -68px;
			z-index: 0;
		}
		.img-4 {
			position: absolute;
			width: 120px;
			bottom: -75px;
			right: -10px;
		}
		.circle {
			position: absolute;
			top: -40px;
			right: -90px;
			height: 60px;
			width: 60px;
			border: 8px solid #ecc5ab;
		}
	}
	.col-5 {
		.subtitle {
			font-size: 12px;
			font-weight: 500;
			letter-spacing: 1px;

			span {
				font-weight: 700;
			}
		}

		.title {
			font-weight: bold;
			font-size: 38px;
		}

		.title-primary {
			font-size: 38px;
			font-weight: 400;
		}
		p {
			font-size: 13px;
			font-weight: 500;
		}
		span {
			font-size: 12px;
			font-weight: 600;

			hr {
				margin: 0;
				padding: 0;
				width: 45%;
				height: 1px;
			}
		}
	}
}
</style>
