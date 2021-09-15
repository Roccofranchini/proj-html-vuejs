<template>
	<div id="app">
		<Header />
		<Main />
		<Footer />
	</div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
	name: "App",
	components: {
		Header,
		Main,
		Footer,
	},
};
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap.scss";
@import "@/assets/scss/style.scss";
@import url("https://fonts.googleapis.com/css2?family=Raleway:ital,wght@0,400;0,500;0,700;1,300&display=swap");
</style>
