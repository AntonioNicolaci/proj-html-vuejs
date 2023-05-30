<script>
import BrandNumber from './BrandNumber.vue';
export default {
    data() {
        return {
            BrandN: [
                {
                    Title:'103K COMMUNITY EARNING',
                    Des:'Distinctively provide acces multfuncto users whereas communicate leveraged services', 
                    Link:'icon-1.png',
                },
                {
                    Title:'34M+ REGISTERED PLAYERS',
                    Des:'Distinctively provide acces multfuncto users whereas communicate leveraged services',
                    Link:'icon-2.png',
                },
                {
                    Title:'240K STRERAMS COMPLETE',
                    Des:'Distinctively provide acces multfuncto users whereas communicate leveraged services',
                    Link:'icon-3.png',
                },
            ]
        }
    },
    components: {
        BrandNumber,
    }
}
</script>
<template>
    <div>
        <img src="../../../public/img/01.png" alt="proTeam" id="proTeam">
        <div>
            <p>
                WHO WE ARE
            </p>
            <h2>
                WE ARE PROFESSIONAL TEAM ESPORT
            </h2>
            <h6>
                Distinctively provide acces mutfuncto users whereas transparent proceses somes ncentivize eficient
                functionalities rather than an extensible archtectur services and cross
            </h6>
            <div>
                <BrandNumber v-for="bn in BrandN"
                :Title="bn.Title"
                :Des="bn.Des"
                :Link="bn.Link" />
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped></style>