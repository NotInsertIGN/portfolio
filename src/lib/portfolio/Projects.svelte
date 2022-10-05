<script lang="ts">
	  import Socials from '../general/Footer.svelte';
    import Navbar from "./Navbar.svelte";

    let home = "nav-element";
    let skills = "nav-element";
    let projects = "nav-element active";
</script>

<Navbar {home} {skills} {projects}></Navbar>

<Socials></Socials>

<div class="content">
    <h1><span style="color:lightcoral">this</span>.<span style="color:#3befff">getProjects()</span>;</h1>
    <p>
        I'm <span style="color:greenyellow">familiar</span> in quite a few programming languages 
        and frameworks, including
        <span style="color:orange">Java</span>,
        <span style="color:yellow">JavaScript</span>
    </p>
</div>

<style>
    @media (min-width: 320px) {
        .content {

        }
    }
    @media (min-width: 1600px) {

    }
    .content {
        position: relative;
        width: clamp(70ch, 50%, 95ch);
        color: #cdddff;
        left: 125px;
    }
    h1 {
        position: relative;
        bottom: 150px;
        font-size: 2.5em;
    }
    p {
        position: relative;
        bottom: 135px;
        font-size: 1.6em;
    }
</style>
