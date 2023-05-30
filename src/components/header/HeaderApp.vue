<script>
import NavbarHeaderApp from './NavbarHeaderApp.vue';

export default {
    components: {
        NavbarHeaderApp,
    }
}
</script>

<template>
    <header>
        <NavbarHeaderApp />
        <!-- jumbo -->   
    </header>
</template>

<style lang="scss" scoped>
    header {
        background: url('../../../public/img/bg.jpg') no-repeat;
        height: 50vw;
    }
</style>