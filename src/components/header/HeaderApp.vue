<script>
import NavbarHeaderApp from './NavbarHeaderApp.vue';
import JumboApp from './JumboApp.vue'

export default {
    components: {
        NavbarHeaderApp,
        JumboApp,
    }
}
</script>

<template>
    <header>
        <NavbarHeaderApp />
        <JumboApp />   
    </header>
</template>

<style lang="scss" scoped>
    header {
        background: url('../../../public/img/bg.jpg') no-repeat;
        height: 950px;
    }
</style>