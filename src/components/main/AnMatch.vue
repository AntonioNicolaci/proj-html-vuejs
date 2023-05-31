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
    <div class="cardAM">
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
            <div class="FMCText">
                <span class="FMCBGame">{{ game }}</span>
                <div>
                    <span class="FMCBData">{{ data }}</span> <span class="FMCBTime">Time: {{ time }}</span>    
                </div>
                <BTNSocialVideo :Vimeo="linkV" :TY="linkYT" :Twitch="linkT" />
            </div>
            <img :src="`../../../public/img/${logoTeam2}`" alt="team-2">
        </div>
    </div>
    <div class="divLL">
        <div class="lungo">
            <div class="largo"></div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.cardAM{
    width: 100%;
}
.FMCHeader {
    display: flex;
    justify-content: space-between;
    background-color: #ff0052;
    padding: 1em 1.5em;
}

.FMCBody {
    display: flex;
    justify-content: space-between;
    background-color: #fff;
    color: #000;
    align-items: center;
    padding: 1em;
    gap: 2em;

    & img {
        padding: 1em;
    }
}

.FMCText {
    display: flex;
    flex-direction: column;
    align-items: center;
    &:last-child {
        padding-top: 1em;
    }
}

.FMCBGame {
    font-weight: bold;
}

.FMCBData {
    padding-right: 1em;
    border-right: 2px solid #999;
}

.FMCBTime {
    padding-left: 1em;
}
.divLL {
    margin-bottom: 2em;
}
</style>