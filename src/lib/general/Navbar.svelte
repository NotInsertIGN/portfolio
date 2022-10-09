<script lang="ts">
    export let home : string;
    export let skills : string;
    export let projects : string;
</script>

<div class="nav">
    <div class={home}>
        <a id="home" href='/'>this.init();</a>
    </div>
    <div class={skills}>
        <a id="skills" href="/skills">this.getSkills();</a>
    </div>
    <div class={projects}>
        <a id="projects" href="/projects">this.getProjects();</a>
    </div>
</div>

<style>
    .nav {
        color: aquamarine;
        font-size: 30px;
        width: 50%;
    }
    .nav-element {
        position: relative;
        top: 2rem;
        left: 95rem;
        width: 15%;
        padding-top: 1.75rem;
        padding-bottom: 1.75rem;
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