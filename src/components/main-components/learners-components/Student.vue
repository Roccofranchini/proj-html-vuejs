<template>
	<div class="col-4">
		<!-- STUDENT STRUCTURE -->

		<div
			id="student"
			class="p-5 mx-2"
			:class="isActive(student.index)"
			@click="$emit('change', index)"
		>
			<h5 class="my-blue student-title mb-3 pe-3">{{ student.title }}</h5>
			<p class="my-gray student-text">{{ student.text }}</p>
			<div class="row">
				<div class="col-2">
					<div class="cornice-img">
						<img
							class="course-img"
							:src="require(`./../../../assets/img/${student.img}.jpg`)"
							alt=""
						/>
					</div>
				</div>
				<div class="col-10 d-flex flex-column justify-content-center">
					<p class="my-blue student-name ms-2 mb-1">{{ student.name }}</p>
					<span class="my-gray ms-2 student-profession"
						>/ {{ student.profession }}</span
					>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "Student",
	props: ["student", "index"],
	methods: {
		isActive(index) {
			return index === true ? "active" : "";
		},
	},
};
</script>

<style scoped lang="scss">
#student {
	background-color: white;
	opacity: 0.4;
}

#student.active {
	opacity: 1;
}

.student-name {
	font-weight: 700;
	font-size: 11px;
}

.student-profession {
	font-weight: 700;
	font-size: 11px;
}

.student-text {
	font-size: 13px;
	font-weight: 600;
}

.student-title {
	font-size: 16px;
	font-weight: 700;
}

.cornice-img {
	height: 50px;
	width: 50px;
	border-radius: 50%;
	overflow: hidden;

	img {
		height: 50px;
	}
}
</style>
