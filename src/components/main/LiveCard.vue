<script>
import ButtonApp from '../ButtonApp.vue';

export default {
    props: {
        text: String,
        img: String,
        link: String,
    },
    components: { ButtonApp }
}
</script>
<template>
    <div>
        <ButtonApp :text="'WATCH NOW'" :link="'#'" :classCSS=[] />
        <h3>{{ text }}</h3>
    </div>
</template>
<style lang="scss" scoped>

</style>