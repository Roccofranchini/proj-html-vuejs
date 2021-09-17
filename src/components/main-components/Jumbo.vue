<template>
	<div id="jumbo">
		<div class="container">
			<div class="row">
				<!-- JUMBOTRON TEXT -->

				<div class="col-6 d-flex align-items-center">
					<div class="jumbo-info px-2">
						<h2 class="fs-1">Distant learning for further expansion</h2>
						<p class="pe-5">
							Learning is a life-long journey that in fact we never find the
							terminate stop. Stop searching, enjoiy the process.
						</p>
						<button class="mt-3 mb-4 button-primary">
							<i class="fas fa-download pe-2"></i> Download free guide
						</button>
						<p>
							Have questions?
							<span class="clickable"
								>Get Free Sample <i class="fas fa-arrow-right"></i>
								<hr
							/></span>
						</p>
					</div>
				</div>
				<!-- JUMBOTRON IMAGES -->

				<div class="col-6 d-flex justify-content-center">
					<div class="images">
						<div class="circle"></div>
						<img
							class="rounded-circle"
							src="../../assets/img/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg"
							alt=""
						/>
						<img
							src="../../assets/img/maxcoach-shape-07-100x100.png"
							alt=""
							class="img-1"
						/>
						<div class="img-2 d-flex flex-column">
							<img
								class="mb-2"
								src="../../assets/img/maxcoach-shape-08.png"
								alt=""
							/>
							<img
								class="mt-2"
								src="../../assets/img/maxcoach-shape-08.png"
								alt=""
							/>
						</div>
						<img
							src="../../assets/img/maxcoach-shape-02.png"
							alt=""
							class="img-3"
						/>
					</div>
				</div>
			</div>
			<!-- PARTNERS LOGOS -->

			<div class="row my-5 partners-logo">
				<div class="col-1"></div>
				<div class="col d-flex align-items-center">
					<img src="..\..\assets\img\client-logo-01.png" alt="" />
				</div>
				<div class="col d-flex align-items-center">
					<img src="..\..\assets\img\client-logo-02.png" alt="" />
				</div>
				<div class="col d-flex align-items-center">
					<img src="..\..\assets\img\client-logo-03.png" alt="" />
				</div>
				<div class="col d-flex align-items-center">
					<img src="..\..\assets\img\client-logo-04.png" alt="" />
				</div>
				<div class="col d-flex align-items-center">
					<img src="..\..\assets\img\client-logo-05.png" alt="" />
				</div>
				<div class="col d-flex align-items-center">
					<img src="..\..\assets\img\client-logo-06.png" alt="" />
				</div>
				<div class="col-1"></div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "jumbo",
};
</script>

<style scoped lang="scss">
//VARS

@import "@/assets/scss/_variables.scss";

//SCSS

#jumbo {
	.jumbo-info {
		h2 {
			font-weight: 700;
			color: $my-blue;
		}
		p {
			font-weight: 600;
			color: $my-gray;
			font-size: 13px;
			line-height: 1.8;

			span {
				color: $my-primary;
				position: relative;
				hr {
					width: 100%;
					position: absolute;
					top: 1px;
					left: 0;
					color: grey;
				}
			}
		}
	}

	.images {
		height: 450px;
		position: relative;

		.rounded-circle {
			width: 450px;
		}

		.img-1 {
			height: 120px;
			position: absolute;
			bottom: 0;
			right: 80px;
			z-index: -1;
		}

		.img-2 {
			position: absolute;
			bottom: 100px;
			left: -70px;
			z-index: -1;
			img {
				height: 100px;
			}
		}

		.circle {
			position: absolute;
			bottom: 100px;
			left: -20px;
		}

		.img-3 {
			height: 100px;
			position: absolute;
			right: -100px;
			top: 100px;
		}
	}

	.partners-logo img {
		max-width: 80px;
		max-height: 60px;
		filter: grayscale(100%) brightness(140%) contrast(100%);
	}
}
</style>
