<script>
import BTNSocialVideo from '../BTNSocialVideo.vue';
export default {
    props: {
        data: String,
        time: String,
        game: String,
        logoTeam1: String,
        logoTeam2: String,
        group: String,
        player: String,
        linkV: String,
        linkYT: String,
        linkT: String,
        linkNow: String,
        pricePool: Number,
    },
    components: {
        BTNSocialVideo,
    }
}
</script>
<template>
    <div>
        <div class="FMCHeader">
            <div>
                <span>{{ group }} GROUP</span>
                <span>{{ player }} PLAYERS</span>
            </div>
            <div>
                <span>PRICE POOl ${{ pricePool }}</span>
            </div>
        </div>
        <div class="FMCBody">
            <img :src="`../../../public/img/${logoTeam1}`" alt="team-1">
            <div>
                <span class="FMCBGame">{{ game }}</span>
                <span class="FMCBData">{{ data }}</span> <span class="FMCBTime">Time: {{ time }}</span>
                <BTNSocialVideo :Vimeo="linkV" :TY="linkYT" :Twitch="linkT" />
            </div>
            <img :src="`../../../public/img/${logoTeam2}`" alt="team-2">
        </div>
    </div>
</template>
<style lang="scss" scoped>
    
</style>