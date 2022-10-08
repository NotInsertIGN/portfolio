<script lang="ts">
	import Skills from '../../lib/portfolio/Skills.svelte';
	import Navbar from "../../lib/general/Navbar.svelte";
	import Footer from "../../lib/general/Footer.svelte";

	const nav = {
		home: "nav-element",
		skills: "nav-element active",
		projects: "nav-element",
	};
</script>

<svelte:head>
	<title>InsertIGN -> Skills</title>
	<meta name="description" content="
	A skills page for InsertIGN, a developer who specializes in web development and Java, where you can find a general overview of his skills and his specializations.">
</svelte:head>

<Navbar {...nav}></Navbar>

<Footer></Footer>

<Skills></Skills>