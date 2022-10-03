<script>
    import Navbar from "./Navbar.svelte";
    import Socials from "../general/Footer.svelte";

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
      although you may know me as<br class="desktop">
      "that one annoying Java developer". I'm fluent in <br class="desktop">
      over 12 programming languages, including
      <span style="color:orange">Java</span>,
      <span style="color: #3b73ff">C++</span>, <br class="desktop">
      <span style="color: rebeccapurple">C#</span>,
      <span style="color:yellow">JavaScript</span>,
      <span style="color: deepskyblue;">Dart</span>,
      <span style="color:blue">Python</span>,
      Ruby and (somewhat!) <br class="desktop">in
      <span style="color:#b30000">Rust</span>. I'm also a huge fan of the
      <span style="color:purple">Linux</span> operating <br class="desktop">
      system, and I use it for a lot of my development. <br class="desktop">
      I'm currently working on a few projects, including <br class="desktop">
      <a href="https://github.com/hypixelapiwrapper/">Neopixel</a>, a group of easy-to-use wrappers for the <br class="desktop">
      Hypixel API, <a href="https://github.com/NotInsertIGN/BiomesRevamped">BiomesRevamped</a>, a group of Minecraft <br class="desktop">
      mods that revamp Minecraft's biomes, and a bunch of <br class="desktop"> random side projects,
      <span style="color: dodgerblue">because what's a true developer <br class="desktop">without them?</span>
    </p>
</div>

<style>
    @media (min-width: 250px) {
      .desktop {
        display:none
      }
    }
    .content {
        position: relative;
        /*width: 50%;*/
        width: clamp(70ch, 50%, 95ch);
        color: #cdddff;
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
