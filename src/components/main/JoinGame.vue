<script>
import ButtonApp from '../ButtonApp.vue';

export default {
    components: { ButtonApp }
}
</script>
<template>
    <div id="JGDiv" class="align">
        <div>
            <p>
                ,ET'S PLAY TOGETHER
            </p>
            <h2>
                JOIN <span>GAMER</span> ESPORTS TO BECOME NEXT PRO GAMER TODAY!
            </h2>
            <p>Distinctively provide acces mutfunct users whereas transparent proceses somes ncentivize eficient functionalities rather than an extensible archtectur services and cross</p>
            <ButtonApp :text="'JOIN COMMUNITY'" :link="'#'" :classCSS=[] />
        </div>
        <img src="../../../public/img/01 (1).png" alt="img">
    </div>
    <div class="divLL">
        <div class="lungo">
            <div class="largo"></div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
    #JGDiv {
        display: flex;
        align-items: center;
        background: url('../../../public/img/bg (4).jpg') no-repeat 50%;

        & div {
            display: flex;
            flex-direction: column;
            row-gap: 1em;
        }
    }
    h2 span {
        color: #ff0052;
    }
    p{
        color: #fff;
    }
</style>