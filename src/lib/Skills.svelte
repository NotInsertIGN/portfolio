<script>
    import Navbar from "./Navbar.svelte";
    import Socials from "./Socials.svelte";

    let home = "nav-element";
    let skills = "nav-element active";
    let projects = "nav-element";
</script>

<Navbar {home} {skills} {projects}></Navbar>

<Socials></Socials>

<div class="content">
    <h1><span style="color:lightcoral">this</span>.<span style="color:#3befff">getSkills()</span>;</h1>
    <p>
        I'm <span style="color:greenyellow">familiar</span> in quite a few programming languages <br>
        and frameworks, including 
        <span style="color:orange">Java</span>,
        <span style="color:yellow">JavaScript</span>
        <br>
    </p>
</div>

<style>
    .content {
        position: relative;
        width: 50%;
        color: rgb(205, 221, 255);
        left: 125px;
    }
    h1 {
        position: relative;
        bottom: 150px;
        font-size: 40px;
    }
    p {
        position: relative;
        bottom: 135px;
        font-size: 25px;
    }
</style>
