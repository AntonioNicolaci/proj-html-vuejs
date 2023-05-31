<script>
import BTNSocialVideo from '../BTNSocialVideo.vue';
import ButtonApp from '../ButtonApp.vue';
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
        ButtonApp,
    }
}
</script>
<template>
    <div id="FSDiv">
        <div class="FMCHeader">
            <div>
                <span>{{ group }} GROUP</span>
                <span>{{ player }} PLAYERS</span>
            </div>
            <div>
                <span>PRICE POOL ${{ pricePool }}</span>
            </div>
        </div>
        <div class="FMCBody">
            <div>
                <span class="FMCBGame">{{ game }}</span>
                <div>
                    <span class="FMCBData">{{ data }}</span> <span class="FMCBTime">Time: {{ time }}</span>
                </div>
            </div>
            <div class="FMImg">
                <img :src="`../../../public/img/${logoTeam1}`" alt="team-1">
                <img src="../../../public/img/vs.png" alt="vs">
                <img :src="`../../../public/img/${logoTeam2}`" alt="team-2">
            </div>
            <div class="FMBTN">
                <BTNSocialVideo :Vimeo="linkV" :TY="linkYT" :Twitch="linkT" />
                <ButtonApp :text="'WATCH NOW'" :link="'#'" :ClassCSS=[] />
            </div>
        </div>
    </div>
    <div class="divLL">
        <div class="lungo">
            <div class="largo"></div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
#FSDiv {
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
    padding: 2em;
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

.FMImg {
    display: flex;
    align-items: center;
    gap: 3em;
}

.FMBTN {
    display: flex;
    align-items: center;
    gap: 1em
}</style>