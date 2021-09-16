<template>
	<div class="background pb-5">
		<section id="tutoring" class="py-5">
			<div class="container">
				<div class="text-center my-5 pb-4">
					<p class="my-gray tutoring-subtitle mb-2">
						MAXCOACH AVAILABLE COURSES
					</p>
					<h3 class="my-blue tutoring-title">
						Acces <span class="my-primary">Smart Tutoring</span> Program for
						Benefits.
					</h3>
				</div>
				<div class="row my-5 pb-5 gx-5">
					<div class="col tutor-card">
						<img src="../../assets/img/home-2-image-box-01.png" alt="" />
						<h4 class="my-blue mt-4 mb-2">Customize Preferences</h4>
						<p class="my-gray">
							Learners are given the rights to arrange and customizee theri
							study schedule and timetable based on preferences.
						</p>
						<span class="my-second-blue"
							>Start here <i class="fas fa-arrow-right"></i
						></span>
					</div>
					<div class="col tutor-card">
						<img src="../../assets/img/about-us-02-image-box-02.png" alt="" />
						<h4 class="my-blue mt-4 mb-2">Cloud Storage</h4>
						<p class="my-gray">
							You can store online lessons via online cloud or download to your
							device and revise lessons on the way.
						</p>
						<span class="my-second-blue"
							>Get Free Quote <i class="fas fa-arrow-right"></i
						></span>
					</div>
					<div class="col tutor-card">
						<img src="../../assets/img/home-2-image-box-03.png" alt="" />
						<h4 class="my-blue mt-4 mb-2">Multimedia Channels</h4>
						<p class="my-gray">
							We provide study materials with various formats: video, audio,
							slides. doc, prints, books and applications.
						</p>
						<span class="my-second-blue"
							>Start now <i class="fas fa-arrow-right"></i
						></span>
					</div>
				</div>
				<div class="row mb-5">
					<div class="col-7 d-flex justify-content-end">
						<div class="images">
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
						</div>
					</div>
					<div class="col-5">
						<div class="text ms-4">
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
								>Download free guidebook <i class="fas fa-arrow-right"></i>
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
};
</script>

<style scoped lang="scss">
@import "@/assets/scss/_variables.scss";

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
		}
	}
}

.row {
	.images {
		position: relative;
		.img-1 {
			max-height: 330px;
		}
		.img-2 {
			position: absolute;
			top: 50%;
			right: 50%;
			transform: translate(50%, -50%);
			height: 50px;
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
