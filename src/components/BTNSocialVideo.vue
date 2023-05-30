<script>
export default {
    props: {
        Vimeo: String,
        YT: String,
        Twitch: String,
    }
}
</script>
<template>
    <div>
        <a :href="Vimeo">
            <img src="../../public/img/social-1.png" alt="vimeo">
        </a>
        <a :href="YT">
            <img src="../../public/img/social-2.png" alt="yt">
        </a>
        <a :href="Twitch">
            <img src="../../public/img/social-3.png" alt="twitch">
        </a>
    </div>
</template>
<style lang="scss" scoped>
    div{
        display: flex;
        gap: 1em;
    }
</style>