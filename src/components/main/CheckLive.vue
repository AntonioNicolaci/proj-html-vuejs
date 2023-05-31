<script>
import LiveCard from './LiveCard.vue';
export default {
    data() {
        return {
            cardLive: [
                {
                    img: '../../../public/img/01.jpg',
                    text: '2022 LVP SUPERLIGA ORANGE SUMMER',
                    link: '#',
                },
                {
                    img: 'https://www.brsoftech.com/blog/wp-content/uploads/2019/11/PUBG-Online-Tournament.jpg',
                    text: 'PUBG CLASSIC TORUNAMENT.',
                    link: '#',
                },
                {
                    img: 'https://www.newsdirect.com/hubfs/best-esports-betting-sites.jpg',
                    text: 'CAN I ADD MY LOCAL BANK...',
                    link: '#',
                },
                {
                    img: 'https://venturebeat.com/wp-content/uploads/2016/03/esl-katowice.jpg?fit=1860%2C1132&strip=all',
                    text: 'LEAUGUE BATTLE TOURNAMENT.',
                    link: '#',
                },
                {
                    img: '../../../public/img/05.jpg',
                    text: 'WHERE CAN I REDEEM MY...',
                    link: '#',
                }
            ]
        }
    },
    components: {
        LiveCard,
    }
}
</script>
<template>
    <div id="CLDiv">
        <p>OUR LATEST VIDEOS</p>
        <h2>CHECK OUR LIVE STREAMING</h2>
        <div class="align">
            <LiveCard v-for="CL in cardLive" :img="CL.img" :text="CL.text" :link="CL.link" />
        </div>
    </div>
</template>
<style lang="scss" scoped>
#CLDiv {
    display: flex;
    flex-direction: column;
    align-items: center;

    & div {
        display: flex;
        flex-wrap: wrap;
    }
}
</style>