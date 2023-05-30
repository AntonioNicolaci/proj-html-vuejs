<script>
export default {
    props: {
        Title: String,
        Des: String,
        Link: String,
    }
}
</script>
<template>
    <div class="BNDiv">
        <div class="BNCircle">
            <img :src="`../../../public/img/${Link}`" :alt="Link">
        </div>
        <div class="BNDText">
            <h3>{{ Title }}</h3>
            <p>{{ Des }}</p>
        </div>
        
    </div>
</template>
<style lang="scss" scoped>
    .BNDiv {
        display: flex;
    }
    .circleBN {
        border-radius: 50%;
        background-color: #ff0052;
    }
    .BNDText {

    }
</style>