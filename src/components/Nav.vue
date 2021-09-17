<template>
	<nav id="nav">
		<div
			class="icons d-flex flex-column align-items-center shadow p-2 mb-5 bg-body rounded"
		>
			<a href=""><i class="fas fa-caret-up ruler"></i></a>
			<a href=""><i class="far fa-life-ring lifering"></i></a>
			<a href=""><i class="fas fa-book"></i></a>
			<a href=""><i class="fas fa-shopping-cart"></i></a>
		</div>
	</nav>
</template>

<script>
export default {
	name: "Nav",
};
</script>

<style scoped lang="scss">
#nav {
	position: fixed;
	top: 150px;
	right: 0;

	.ruler {
		font-size: 17px;
		margin-bottom: 0;
	}

	.life-ring {
		margin-top: 0;
	}

	a {
		text-decoration: none;
		color: black;
		font-size: 13px;
		margin: 3px;

		i {
			transition: transform;
		}

		i:hover {
			transform: scale(1.5);
		}
	}
}
</style>
