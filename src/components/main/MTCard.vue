<script>
import BTNSocialVideo from '../BTNSocialVideo.vue';

export default {
    data() {
        return {
            // linkBG: `../../../public/img/${bgLink}'`
        }
    },
    props: {
        link: String,
        nameTeam: String,
        bgLink: String,
        Vimeo: String,
        YT: String,
        Twitch: String,
    },
    components: { BTNSocialVideo }
}
</script>
<template>
    <div class="MTD">
        <img :src="`../../../public/img/${link}`" alt="logoTeam">
        <h3>{{ nameTeam }}</h3>
        <BTNSocialVideo :Vimeo="Vimeo" :YT="YT" :Twitch="Twitch" />
    </div>
</template>
<style lang="scss" scoped>
.MTD {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 1em;
    width: calc(100% / 5 - 1em);
    height: 350px;
    position: relative;
    border: 10px solid #232a5c;
    padding: 1em;
}

img {
    width: 102px;
    height: 100px;
}
</style>