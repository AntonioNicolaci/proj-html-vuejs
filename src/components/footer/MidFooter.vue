<script>
import BTNSocialVideo from '../BTNSocialVideo.vue';
import ButtonApp from '../ButtonApp.vue';
import JPCard from './JPCard.vue';
export default {
    data() {
        return {
            JPCard: [
                {
                    logo:'01 (4).jpg',
                    nameG:'FREE POKER GAME',
                    poker:230,
                    rating:5,
                },
                {
                    logo:'01 (4).jpg',
                    nameG:'CLUB POKER GAME',
                    poker:290,
                    rating:5,
                },
                {
                    logo:'01 (4).jpg',
                    nameG:'ROYAL POKER GAME',
                    poker:330,
                    rating:5,
                },
            ]
        }
    },
    components: {
        BTNSocialVideo,
        JPCard,
        ButtonApp,
    }
}
</script>
<template>
    <div>
        <img src="../../../public/img/logo.png" alt="logo">
        <p>
            Upropriate brand economca sound technolog after covalent technology enable prospective wastng markets whereas propriate and brand economca sound technolog
        </p>
        <BTNSocialVideo :Vimeo="'#'" :YT="'#'" :Twitch="'#'" />
    </div>
    <div>
        <h2>TOP JACKPOT GAMES</h2>
        <JPCard v-for="JPC in JPCard" :logo="JPC.logo" :nameG="JPC.nameG" :poker="JPC.poker" :rating="JPC.rating"/>
    </div>
    <div>
        <h2>OUR NEWSLETTER</h2>
        <p>Gamer esports organization supported by community leaders</p>
        <input type="text">
        <input type="text">
        <ButtonApp :text="'SEND MASSAGE'" :link="'#'" :classCSS=[] />
    </div>
</template>
<style lang="scss" scoped>
    
</style>