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
    display: flex;
    flex-direction: column;
    align-items: center;
    color: #fff;
}

#upFooter {
    display: flex;
    justify-content: center;
    width: 100%;
    border-bottom: 1px solid rgba(100, 100, 100, 0.5);
}

#botFooter {
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #232a5c;
    width: 100%;
    height: 5em;
}
</style>