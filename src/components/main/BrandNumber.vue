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
        margin-bottom: 1em;
    }
    .BNCircle {
        border-radius: 50%;
        background-color: #ff0052;
        padding: 1em;
        margin-right: 1em;
        width: calc(36px + 2em) ;
        height: calc(36px + 2em);
    }
    .BNDText {
        display: flex;
        flex-direction: column;
        row-gap: 1em;
        
        & p {
            color: #fff;
        }
    }
</style>