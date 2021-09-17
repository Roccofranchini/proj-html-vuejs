<template>
	<!-- CARD STRUCTURE -->

	<div class="col-6">
		<div class="single-card py-4 px-3 clickable">
			<div class="row">
				<div class="col-4">
					<div class="cornice-img">
						<img
							class="course-img"
							:src="require(`./../../../assets/img/${course.img}.jpg`)"
							alt=""
						/>
					</div>
				</div>
				<div class="col-8">
					<p class="mb-1">{{ this.course.price }}</p>
					<h6>{{ this.course.title }}</h6>
					<span class="mx-2"
						><i class="far fa-file-alt mx-1"></i>
						{{ this.course.lessons }} Lessons
					</span>
					<span class="mx-2"
						><i class="far fa-user mx-1"></i>
						{{ this.course.students }} Students</span
					>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "Card",
	props: ["course"],
};
</script>

<style scoped lang="scss">
//VARS

@import "@/assets/scss/_variables.scss";

//SCSS

.single-card:hover {
	background-color: white;
}

p {
	color: $my-primary;
	font-family: "Roboto", sans-serif;
	font-size: 25px;
	font-weight: bold;
}

h6 {
	color: $my-blue;
	font-weight: 600;
}

span {
	color: $my-gray;
	font-size: 12px;
}

.cornice-img {
	height: 130px;
	width: 130px;
	border-radius: 50%;
	overflow: hidden;
}

.cornice-img img {
	width: 240px;
	object-position: center;
}
</style>
