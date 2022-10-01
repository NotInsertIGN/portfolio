<script>
    export let home;
    export let skills;
    export let projects;
</script>

<div class="nav">
    <div class={home}>
        <!-- <Link to="/">this.getSummary();</Link> -->
        <a id="home" href="/">this.init();</a>
    </div>
    <div class={skills}>
        <!-- <Link to="skills">this.getSkills();</Link> -->
        <a id="skills" href="/skills">this.getSkills();</a>
    </div>
    <div class={projects}>
        <!-- <Link to="projects">this.getProjects();</Link> -->
        <a id="projects" href="/projects">this.getProjects();</a>
    </div>
</div>

<style>
    .nav {
        font-family: "Courier 10 Pitch", monospace;
        color: aquamarine;
        font-size: 30px;
        width: fit-content;
    }
    .nav-element {
        position: relative;
        top: 25px;
        left: 1525px;
        width: 15%;
        padding-top: 25px;
        padding-bottom: 25px;
    }
    .active {
        text-decoration: line-through;
    }
    a {
        color: #3befff;
        text-decoration: none;
    }
    a:hover {
        text-decoration: underline cadetblue;
    }
</style>