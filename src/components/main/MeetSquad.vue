<script>
import MTCard from './MTCard.vue';
export default {
    data() {
        return {
            SquadObj: [
                {
                    link: 'team-2.png',
                    nameTeam: 'GAMING TEAM',
                    bgLink: '5.jpg',
                    linkVimeo: '#',
                    linkYT: '#',
                    linkTwitch: '#'
                },
                {
                    link: 'teamsm-1.png',
                    nameTeam: 'DRAGON TEAM',
                    bgLink: '1.jpg',
                    linkVimeo: '#',
                    linkYT: '#',
                    linkTwitch: '#'
                },
                {
                    link: 'teamsm-4.png',
                    nameTeam: 'MONKEY TEAM',
                    bgLink: '5.jpg',
                    linkVimeo: '#',
                    linkYT: '#',
                    linkTwitch: '#'
                },
                {
                    link: 'teamsm-2.png',
                    nameTeam: 'WOLVES TEAM',
                    bgLink: '1.jpg',
                    linkVimeo: '#',
                    linkYT: '#',
                    linkTwitch: '#'
                },
                {
                    link: 'teamsm-7.png',
                    nameTeam: 'ROBOTO TEAM',
                    bgLink: '5.jpg',
                    linkVimeo: '#',
                    linkYT: '#',
                    linkTwitch: '#'
                },
            ]
        }
    },
    components: {
        MTCard,
    }
}
</script>
<template>
    <div id="MTSDiv">
        <p>
            UOR TEAM PLAYERS
        </p>
        <h2>
            MEET OUR SQUAD PLAYERS
        </h2>
        <div id="MTCD">
            <MTCard v-for="SOBJ in SquadObj" :link="SOBJ.link" :nameTeam="SOBJ.nameTeam" :bgLink="SOBJ.bgLink"
                :Vimeo="SOBJ.linkVimeo" :YT="SOBJ.linkYT" :Twitch="SOBJ.linkTwitch" />
        </div>
    </div>
</template>
<style lang="scss" scoped>
#MTSDiv {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 1em;
    margin-block: 6em;
}

#MTCD {
    display: flex;
    gap: 1em;
}
</style>