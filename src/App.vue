<script>
import AppMain from "./components/AppMain.vue"
import AppFooter from "./components/AppFooter.vue"
import AppHeader from "./components/AppHeader.vue"



import axios from 'axios'; //importo Axios
import { store } from "./store.js" //state management

export default {
	components: {
		AppHeader,
		AppMain,
		AppFooter
	},
	data() {
		return {
			store,
			navLinks: [
				{
					text: "Home", link: "#"
				},
				{
					text: "Services", link: "#"
				},
				{
					text: "About", link: "#"
				},
				{
					text: "Videos", link: "#"
				},
				{
					text: "Blog", link: "#"
				},
				{
					text: "Store", link: "#"
				},
			],

			postsLinks: [
				{
					text: ">The best protein shake", link: "#"
				},
				{
					text: ">Ultimate cardio workout", link: "#"
				},
				{
					text: ">New juices available now", link: "#"
				},
				{
					text: ">Tips to find trainng partners", link: "#"
				},
				{
					text: ">20 best healthy recipes", link: "#"
				},

			]
		}
	},
	mounted() {
		this.doThings();

		// axios.get("indirizzo").then(risultato => {
		// 	console.log(risultato);
		// }).catch(errore => {
		// 	console.error(errore);
		// });
	},
	methods: {
		doThings() {
			console.log("App.vue does things");
		}
	}
}
</script>

<template>
	<header>
		<AppHeader :navBarLinks="navLinks" />
	</header>
	<main>
		<AppMain />
	</main>
	<footer>
		<AppFooter :postsLinkList="postsLinks" />
	</footer>
</template>


<style lang="scss">
// importo il foglio di stile generale dell'applicazione, non-scoped
@use './styles/general.scss';
</style>

<style scoped lang="scss">
// importo variabili
// @use './styles/partials/variables' as *;

header {
	height: 6rem;
	padding-top: 0.4rem;
}

main {}

footer {
	margin-top: 2rem;
}
</style>