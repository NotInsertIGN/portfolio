<script lang="ts">
	import Projects from '../../lib/portfolio/Projects.svelte';
	import Navbar from "../../lib/general/Navbar.svelte";
	import Footer from "../../lib/general/Footer.svelte";

	const nav = {
		home: "nav-element",
		skills: "nav-element",
		projects: "nav-element active",
	};
</script>

<svelte:head>
	<title>InsertIGN -> Projects</title>
	<meta name="description" content="
	A projects page for InsertIGN, a developer who specializes in web development and Java, where you can find a general overview of his many projects related to numerous fields like web development and software development.">
</svelte:head>

<Navbar {...nav}></Navbar>

<Footer></Footer>

<Projects></Projects>