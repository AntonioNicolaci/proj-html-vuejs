<script>
import ButtonApp from '../ButtonApp.vue';
import FirstMatch from './FirstMatch.vue';
import AnMatch from './AnMatch.vue';

export default {
    data() {
        return {
            allMatch: [
                {
                    data: '30 April 2022',
                    time: '08:30PM',
                    game: 'BATTLEFIELD-4 TOURNAMENT',
                    team1: '',
                    logoTeam1: 'teamsm-6.png',
                    team2: '',
                    logoTeam2: 'teamsm-9.png',
                    group: '2',
                    player: '32',
                    linkV: '#',
                    linkYT: '#',
                    linkT: '#',
                    linkNow: '#',
                    pricePool: 3200,
                },
                {
                    data: '30 April 2022',
                    time: '08:30PM',
                    game: 'BATTLEFIELD-4 TOURNAMENT',
                    team1: '',
                    logoTeam1: 'teamsm-1.png',
                    team2: '',
                    logoTeam2: 'teamsm-2.png',
                    group: '2',
                    player: '32',
                    linkV: '#',
                    linkYT: '#',
                    linkT: '#',
                    linkNow: '#',
                    pricePool: 3200,
                },
                {
                    data: '30 April 2022',
                    time: '08:30PM',
                    game: 'BATTLEFIELD-4 TOURNAMENT',
                    team1: '',
                    logoTeam1: 'teamsm-3.png',
                    team2: '',
                    logoTeam2: 'teamsm-4.png',
                    group: '2',
                    player: '32',
                    linkV: '#',
                    linkYT: '#',
                    linkT: '#',
                    linkNow: '#',
                    pricePool: 3200,
                },
                {
                    data: '30 April 2022',
                    time: '08:30PM',
                    game: 'BATTLEFIELD-4 TOURNAMENT',
                    team1: '',
                    logoTeam1: 'teamsm-5.png',
                    team2: '',
                    logoTeam2: 'teamsm-6.png',
                    group: '2',
                    player: '32',
                    linkV: '#',
                    linkYT: '#',
                    linkT: '#',
                    linkNow: '#',
                    pricePool: 3200,
                },
                {
                    data: '30 April 2022',
                    time: '08:30PM',
                    game: 'BATTLEFIELD-4 TOURNAMENT',
                    team1: '',
                    logoTeam1: 'teamsm-7.png',
                    team2: '',
                    logoTeam2: 'teamsm-8.png',
                    group: '2',
                    player: '32',
                    linkV: '#',
                    linkYT: '#',
                    linkT: '#',
                    linkNow: '#',
                    pricePool: 3200,
                },
                {
                    data: '30 April 2022',
                    time: '08:30PM',
                    game: 'BATTLEFIELD-4 TOURNAMENT',
                    team1: '',
                    logoTeam1: 'teamsm-9.png',
                    team2: '',
                    logoTeam2: 'teamsm-10.png',
                    group: '2',
                    player: '32',
                    linkV: '#',
                    linkYT: '#',
                    linkT: '#',
                    linkNow: '#',
                    pricePool: 3200,
                },
                {
                    data: '30 April 2022',
                    time: '08:30PM',
                    game: 'BATTLEFIELD-4 TOURNAMENT',
                    team1: '',
                    logoTeam1: 'teamsm-11.png',
                    team2: '',
                    logoTeam2: 'teamsm-12.png',
                    group: '2',
                    player: '32',
                    linkV: '#',
                    linkYT: '#',
                    linkT: '#',
                    linkNow: '#',
                    pricePool: 3200,
                },
            ]
        }
    },
    components: { ButtonApp, FirstMatch, AnMatch }
}
</script>
<template>
    <div id="AllMDiv" class="align">
        <p>
            ANYWHERE, ANYTINE
        </p>
        <h2>
            ALL MATCHES SCHEDULE
        </h2>
        <FirstMatch :data="allMatch[0].data" :time="allMatch[0].time" :game="allMatch[0].game"
            :logoTeam1="allMatch[0].logoTeam1" :logoTeam2="allMatch[0].logoTeam2" :group="allMatch[0].group"
            :player="allMatch[0].player" :linkV="allMatch[0].linkV" :linkYT="allMatch[0].linkYT" :linkT="allMatch[0].linkT"
            :linkNow="allMatch[0].linkNow" :pricePools="allMatch[0].pricePool" />
        <div id="ANMatchDiv">
            <div>
                <h3>UPCOMIC MATCHES</h3>
                <AnMatch v-for="n in 3" :data="allMatch[n].data" :time="allMatch[n].time" :game="allMatch[n].game"
                    :logoTeam1="allMatch[n].logoTeam1" :logoTeam2="allMatch[n].logoTeam2" :group="allMatch[n].group"
                    :player="allMatch[n].player" :linkV="allMatch[n].linkV" :linkYT="allMatch[n].linkYT"
                    :linkT="allMatch[n].linkT" :linkNow="allMatch[n].linkNow" :pricePools="allMatch[n].pricePool" />
            </div>
            <div>
                <h3>PREVIOUS MATCHES</h3>
                <AnMatch v-for="n in 3" :data="allMatch[n + 3].data" :time="allMatch[n + 3].time" :game="allMatch[n + 3].game"
                    :logoTeam1="allMatch[n + 3].logoTeam1" :logoTeam2="allMatch[n + 3].logoTeam2" :group="allMatch[n + 3].group"
                    :player="allMatch[n + 3].player" :linkV="allMatch[n + 3].linkV" :linkYT="allMatch[n + 3].linkYT"
                    :linkT="allMatch[n + 3].linkT" :linkNow="allMatch[n + 3].linkNow" :pricePools="allMatch[n + 3].pricePool" />
            </div>
        </div>
        <ButtonApp :text="'BROWSER ALL MATCHES'" :link="'#'" :classCSS="[]" />
    </div>
</template>
<style lang="scss" scoped>
#AllMDiv {
    display: flex;
    flex-direction: column;
    align-items: center;

    & h3{
        margin-block: 6em 2em;
    }
}
#ANMatchDiv {
    display: flex;
    justify-content: center;
    width: 100%;
    gap: 2em;
    & div{
        text-align: center;
    }
}
</style>