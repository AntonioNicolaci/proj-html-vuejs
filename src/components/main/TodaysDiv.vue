<script>
import ButtonApp from '../ButtonApp.vue';
import TodayCard from './TodayCard.vue';
export default {
    data() {
        return {
            todayArr: [
                {
                    team1: 'team-1.png',
                    team2: 'team-2.png',
                },
                {
                    team1: 'teamsm-4.png',
                    team2: 'teamsm-3.png',
                },
                {
                    team1: 'teamsm-2.png',
                    team2: 'teamsm-1.png',
                },
            ]
        }
    },
    components: {
        ButtonApp,
        TodayCard,
    }
}
</script>
<template >
    <div class="mainBorderCard">
        <p>
            TODAY'S
        </p>
        <h2>
            OUR GAME COLLECTION
        </h2>
        <div class="todayCardDiv">
            <TodayCard v-for="today in todayArr" :team1="today.team1" :team2="today.team2" />
        </div>
        <ButtonApp :text="'BROWSER ALL GAMES'" :link="'#'" classBTN='' />
    </div>
</template>
<style lang="scss" scoped>
.todayCardDiv {
    display: flex;
    flex-direction: row;
}
</style>