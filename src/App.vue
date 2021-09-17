<template>
	<div id="app">
		<Header />
		<Nav />
		<Main />
		<Footer />
	</div>
</template>

<script>
import Header from "./components/Header.vue";
import Nav from "./components/Nav.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
	name: "App",
	components: {
		Header,
		Nav,
		Main,
		Footer,
	},
};
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap.scss";
@import "@/assets/scss/style.scss";
@import url("https://fonts.googleapis.com/css2?family=Raleway:wght@300;400;500;600;700;800&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700;900&display=swap");
#app .container {
	max-width: 1000px;
	margin: auto;
}
</style>
