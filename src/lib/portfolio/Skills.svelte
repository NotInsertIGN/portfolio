<script lang="ts">
    import Navbar from "./Navbar.svelte";
    import Socials from "../general/Footer.svelte";

    let home = "nav-element";
    let skills = "nav-element active";
    let projects = "nav-element";
</script>

<Navbar {home} {skills} {projects}></Navbar>

<Socials></Socials>

<div class="content">
    <h1><span style="color:lightcoral">this</span>.<span style="color:#3befff">getSkills()</span>;</h1>
    <p>
        I'm <span style="color:greenyellow">familiar</span> in quite a few programming languages 
        and frameworks, including
        <span style="color:orange">Java</span>,
        <span style="color: #3b73ff">C++</span>,
        <span style="color: rebeccapurple">C#</span>,
        <span style="color:yellow">JavaScript</span>,
        <span style="color: deepskyblue;">Dart</span>,
        <span style="color:lightseagreen">Python</span>,
        <span style="color: orangered;">Ruby</span> and (somewhat!) in
        <span style="color:#b30000">Rust</span>. I'm also 
        <span style="color: purple">well-acquainted</span> with
        <span style="color: aquamarine">web development</span>, along with 
        many different <span style="color: cornflowerblue;">frameworks</span>, such as
        <span style="color: crimson">SvelteKit</span>,
        <span style="color: antiquewhite">NextJS</span>,
        <span style="color: seagreen;">NuxtJS</span>, and
        <span style="color: forestgreen">SpringBoot</span>.
        I
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
