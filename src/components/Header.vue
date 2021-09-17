<template>
	<header>
		<div id="nav" class="h-100">
			<div class="container h-100">
				<div class="row align-items-center h-100">
					<!-- LOGO -->

					<div class="col-3">
						<img class="clickable" src="../assets/img/dark-logo.png" alt="" />
					</div>
					<!-- MENU' -->

					<div class="col-6">
						<ul class="d-flex justify-content-between m-0 py-0 px-3">
							<li v-for="(link, index) in links" :key="index">
								<a href="">{{ link }} <i class="fas fa-angle-down"></i></a>
							</li>
						</ul>
					</div>
					<!-- SEARCHBAR -->

					<div class="col-3 ">
						<div class="searchbar">
							<i class="far fa-user-circle pe-3"></i>
							<input type="text" placeholder="Search.." />
							<i class="fas fa-search"></i>
						</div>
					</div>
				</div>
			</div>
		</div>
	</header>
</template>

<script>
export default {
	name: "Header",
	data() {
		return {
			links: ["Home", "Pages", "Courses", "Features", "Blog", "Shop"],
		};
	},
};
</script>

<style scoped lang="scss">
//VARS
@import "@/assets/scss/_variables.scss";

//SCSS

header {
	height: 70px;
	box-shadow: 0 3px rgba(236, 236, 236, 0.349);

	img {
		height: 20px;
	}
	li {
		font-size: 13px;
		font-weight: 500;
		a {
			text-decoration: none;
			color: black;
		}
	}

	li:hover {
		transform: scale(1.1);
	}

	.searchbar {
		position: relative;
		input {
			background-color: #f5f5f5;
			border: 0;
			border-radius: 5px;
			font-size: 12px;
			padding: 10px 16px;
		}
		i {
			font-size: 14px;
		}
		.fa-search {
			color: $my-primary;
			position: absolute;
			left: 180px;
			top: 10px;
		}
	}
}
</style>
