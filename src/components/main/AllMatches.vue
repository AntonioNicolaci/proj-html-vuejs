<script>
import ButtonApp from '../ButtonApp.vue';

export default {
    components: { ButtonApp }
}
</script>
<template>
    <div>
        <p>
            ANYWHERE, ANYTINE
        </p>
        <h2></h2>
        <FirstMatch />
        <div>
            <div>
                <h3></h3>
                <AnMatch />
            </div>
            <div>
                <h3></h3>
                <AnMatch />
            </div>
        </div>
        <ButtonApp
        :text="'BROWSER ALL MATCHES'"
        :link="'#'"
        :classCSS="[]" />
    </div>
</template>
<style lang="scss" scoped>
    
</style>