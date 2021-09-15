<template>
	<header>
		<div class="container h-100">
			<div class="row align-items-center h-100">
				<div class="col-3">
					<img src="../assets/img/dark-logo.png" alt="" />
				</div>
				<div class="col-6">
					<ul class="d-flex justify-content-between m-0 py-0 px-3">
						<li v-for="(link, index) in links" :key="index">
							{{ link }} <i class="fas fa-angle-down"></i>
						</li>
					</ul>
				</div>
				<div class="col-3">
					<div class="searchbar">
						<input class="py-1 ps-2" type="text" placeholder="Search.." />
						<i class="fas fa-search"></i>
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
@import "@/assets/scss/_variables.scss";

header {
	height: 50px;
	box-shadow: 0 2px rgba(211, 211, 211, 0.349);
	img {
		height: 20px;
	}

	.searchbar {
		position: relative;
		input {
			background-color: #f5f5f5;
			border: 0;
			border-radius: 5px;
		}
		i {
			color: $my-green;
			position: absolute;
			left: 150px;
			top: 8px;
		}
	}
}
</style>
