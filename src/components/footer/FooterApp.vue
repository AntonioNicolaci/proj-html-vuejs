<script>
import UpFooter from './UpFooter.vue';
import MidFooter from './MidFooter.vue';
import BotFooter from './BotFooter.vue';
export default {
    components: {
        UpFooter,
        MidFooter,
        BotFooter,
    }
}
</script>
<template>
    <footer>
        <div id="upFooter">
            <UpFooter />
        </div>
        <div id="midFooter">
            <MidFooter />
        </div>
        <div id="botFooter">
            <BotFooter />
        </div>
    </footer>
</template>
<style lang="scss" scoped>
    footer {
        background: url('../../../public/img/bg (3).jpg');
    }
</style>