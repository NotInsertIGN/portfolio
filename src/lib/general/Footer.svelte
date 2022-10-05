<script>
    import Giscus from "$lib/giscus/Giscus.svelte";
</script>

<div class="footer">
    <div class="socials">
        <div class="social">
            <a href="https://www.github.com/notinsertign"><img src="/socials/github.webp" alt="github" width=32 height=30></a>
        </div>
        <div class="social">
            <a href="https://www.discord.gg/zZjPsPt2vy"><img src="/socials/discord.webp" alt="discord" width=30 height=23></a>
        </div>
        <div class="social">
            <a href="https://www.twitter.com/lolitsinsert"><img src="/socials/twitter.webp" alt="twitter" width=30 height=24></a>
        </div>
        <div class="social">
            <a href="https://www.youtube.com/channel/UCqZb6n_MaQbVE2iS93dTZgA"><img src="/socials/youtube.webp" alt="youtube" width=30 height=20></a>
        </div>
    </div>
    <div class="description">
        <span class="description-item">Made with <span style="color: crimson">love️</span>
            by <span style="color: greenyellow">InsertIGN</span></span>
    </div>
</div>

<style>
    .socials {
        min-width: 100px;
        height: 30px;
        display: flex;
        justify-content: center;
    }
    .social {
        min-width: 100px;
        position: relative;
        padding: 25px;
        top: 500px;
        right: 20px;
    }
    .description {
        position: relative;
        color: white;
        display: flex;
        justify-content: flex-start;
    }
    .description-item {
        position: relative;
        min-width: 100px;
        padding-left: 25px;
        padding-right: 25px;
        top: 31.5em;
    }
</style>