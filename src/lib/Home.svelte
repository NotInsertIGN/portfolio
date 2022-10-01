<script>
    import Navbar from "./Navbar.svelte";
    import Socials from "./Socials.svelte";

    let home = "nav-element active";
    let skills = "nav-element";
    let projects = "nav-element";
</script>

<Navbar {home} {skills} {projects}></Navbar>

<Socials></Socials>

<div class="content">
    <h1>System.out.println("<span style="color:#3befff">Hello world!</span>");</h1>
    <p>
        <span style="color:red">Hey!</span> I'm <span style="color:greenyellow">InsertIGN</span>, 
        although you may know me as<br>
       "that one annoying Java developer". I'm fluent in <br>
        over 12 programming languages, including <span style="color:orange">Java</span>, C++, <br>
        C#, <span style="color:yellow">JavaScript</span>, Dart, 
        <span style="color:blue">Python</span>, Ruby and (somewhat!) <br>
        <span style="color:#b30000">Rust</span> I'm also a huge fan of the <span style="color:purple">Linux</span> operating <br>
        system, and I use it for a lot of my development. <br>
        I'm currently working on a few projects, including <br>
        <a href="https://github.com/hypixelapiwrapper/">Neopixel</a>, a group ofeasy-to-use wrappers for the <br>
        Hypixel API, <a href="https://github.com/NotInsertIGN/BiomesRevamped">BiomesRevamped</a>, a group of Minecraft <br>
        mods that revamp Minecraft's biomes, and a bunch of <br> random side projects,
        <span style="color:#3b73ff">because what's a true developer <br>without them?</span>
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
