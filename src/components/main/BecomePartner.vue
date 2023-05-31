<script>
import ButtonApp from '../ButtonApp.vue';
export default {
    data() {
        return {
            partner: [
                {
                    namePartner:'P-sky',
                    logoPartner:'07.png',
                },
                {
                    namePartner:'Vita-di-P',
                    logoPartner:'08.png',
                },
                {
                    namePartner:'P-ndemonic',
                    logoPartner:'06.png',
                },
                {
                    namePartner:'P-fuel',
                    logoPartner:'05.png',
                },
                {
                    namePartner:'P-ndemonic',
                    logoPartner:'06.png',
                },
                {
                    namePartner:'P-sky',
                    logoPartner:'07.png',
                },
                {
                    namePartner:'Vita-di-P',
                    logoPartner:'08.png',
                },
                {
                    namePartner:'Fire-P',
                    logoPartner:'05.png',
                },
            ]
        }
    },
    components: {
        ButtonApp,
    }
}
</script>
<template>
    <div id="BPDiv">
        <p>WE ARE PARTNERS</p>
        <h2>BECOME A PARTNER OF GAME</h2>
        <div id="DivImg" class="align">
            <img v-for="PT in partner" :src="`../../../public/img/${PT.logoPartner}`" :alt="PT.namePartner">
        </div>
        <ButtonApp :text="'BECOME A PARTNER'" :link="'#'" :classCSS=[] />
    </div>
</template>
<style lang="scss" scoped>
    #BPDiv {
        display: flex;
        align-items: center;
        flex-direction: column;
        row-gap: 1em;
        & p {
            padding-top: 6em;
        }
    }
    #DivImg {
        display: flex;
        flex-wrap: wrap;
        gap: 2em;
        justify-content: center;
        padding-block: 1em;
    }
</style>