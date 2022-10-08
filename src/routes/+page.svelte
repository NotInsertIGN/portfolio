<script lang="ts">
	import Home from '../lib/portfolio/Home.svelte';
	import Footer from "../lib/general/Footer.svelte";
	import Navbar from '../lib/general/Navbar.svelte';

	const nav = {
		home: "nav-element active",
		skills: "nav-element",
		projects: "nav-element",
	};
</script>

<svelte:head>
	<title>InsertIGN -> Home</title>
	<meta name="description" content="
	A home page for InsertIGN, a developer who specializes in web development and Java, where you can find a general overview of his programming career.">
</svelte:head>

<Navbar {...nav}></Navbar>

<Footer></Footer>

<Home></Home>