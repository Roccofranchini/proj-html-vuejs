<template>
	<footer>
		<section id="top-footer" class="pb-5">
			<div class="container my-5">
				<div class="row">
					<div class="col-2 d-flex align-items-end">
						<div class="circle mb-5"></div>
					</div>
					<div class="col-8">
						<div
							class="subscribe-text px-5 d-flex flex-column align-items-center mt-5"
						>
							<h4 class="my-blue pt-3 pb-2 title">
								Subscribe <span class="my-primary">Newsletter</span>
							</h4>
							<p class="my-gray mb-5  px-4 text-center">
								Enter your email adress to register to our new newsletter
								subscription delivered on a regular basis!
							</p>
							<div class="input-group mb-3">
								<input
									type="text"
									class="form-control my-gray"
									placeholder="Enter your email"
									aria-label="Enter your email"
									aria-describedby="button-addon2"
								/>
								<button
									class="btn btn-outline-secondary button-primary"
									type="button"
									id="button-addon2"
								>
									Subscribe
								</button>
							</div>
						</div>
					</div>
					<div
						class="col-2 d-flex flex-column align-items-end position-relative"
					>
						<img
							class="pt-5 grid-decoration"
							src="../assets/img/maxcoach-shape-09.png"
							alt=""
						/>
						<img
							class="pt-5 coach-circle"
							src="../assets/img/maxcoach-shape-02.png"
							alt=""
						/>
					</div>
				</div>
			</div>
		</section>
		<section id="bottom-footer" class="pt-5">
			<div class="container pt-5">
				<div class="row">
					<div class="col-6 contacts">
						<p>Address</p>
						<ul class="ps-0">
							<li>382 NE 191stSt # 87394 Miami, FL 33179-3899</li>
							<li>+1 (305) 547-9909 (9am - 5pm, EST, Monday - Friday)</li>
							<li>support@maxcoach.com</li>
						</ul>
						<a href=""><i class="fab fa-facebook-square"></i></a
						><a href=""><i class="fab fa-twitter"></i></a
						><a href=""><i class="fab fa-instagram"></i></a
						><a href=""><i class="fab fa-linkedin"></i></a>
					</div>
					<div class="col-6 d-flex">
						<div class="col-3">
							<p class="pt-2">Explore</p>
							<ul class="ps-0">
								<li>Start here</li>
								<li>Blog</li>
								<li>About us</li>
							</ul>
						</div>
						<div class="col-3">
							<ul class="ps-0 pt-5">
								<li>Start here</li>
								<li>Blog</li>
								<li>About us</li>
							</ul>
						</div>
						<div class="col-3">
							<p class="pt-2">Information</p>
							<ul class="ps-0">
								<li>Membership</li>
								<li>Purchase guide</li>
								<li>Privacy policy</li>
								<li>Terms of services</li>
							</ul>
						</div>
					</div>
				</div>
				<p class="text-center pt-5 pb-3 copyright">
					@ 2020 Maxcoach. All Rights Reserved
				</p>
				<button class="button-primary">
					<a href="#"><i class="fas fa-arrow-up"></i></a>
				</button>
			</div>
		</section>
	</footer>
</template>

<script>
export default {
	name: "Footer",
};
</script>

<style scoped lang="scss">
@import "@/assets/scss/_variables.scss";

#top-footer {
	.circle {
		border-color: $my-primary;
	}

	.subscribe-text {
		p {
			font-size: 14px;
			font-weight: 600;
		}

		input {
			border: 0;
			background-color: #f5f7fa;
			font-size: 13px;
		}
	}

	.grid-decoration {
		height: 200px;
	}

	.coach-circle {
		position: absolute;
		bottom: 10px;
		right: 5px;
		width: 100px;
	}
}

#bottom-footer {
	background-color: #f8f8f8;
	position: relative;

	p {
		font-weight: 700;
		font-size: 14px;
	}

	li {
		font-size: 12px;
		font-weight: 600;
		color: gray;
		padding: 5px 0;
	}

	a {
		color: $my-gray;
		padding: 0 10px;
		font-size: 18px;
	}

	.copyright {
		color: $my-gray;
		font-size: 12px;
		font-weight: 600;
	}

	button {
		padding: 10px 10px;
		border-radius: 50%;
		position: absolute;
		bottom: 20px;
		right: 20px;
		a {
			color: white;
			text-decoration: none;
			transition: padding 1s;
		}

		a:hover {
			padding: 13px 13px;
		}
	}
}
</style>
