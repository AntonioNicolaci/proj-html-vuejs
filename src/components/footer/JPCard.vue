<script>
import { BIconStar, BIconStarFill } from 'bootstrap-icons-vue';
export default {
    props: {
        logo: String,
        nameG: String,
        poker: Number,
        rating: Number,
    },
    components: {
        BIconStar,
        BIconStarFill,
    }
}
</script>
<template>
    <div class="JPCDiv">
        <img :src="`../../../public/img/${logo}`" :alt="logo">
        <div class="JPCDText">
            <h3>{{ nameG }}</h3>
            <p>Poker: ${{ poker }}</p>
            <div>
                <template v-for="n in 5">
                    <BIconStarFill v-if="rating >= n" />
                    <BIconStar v-else />
                </template>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.JPCDiv{
    display: flex;
    align-items: center;
    width: 100%;
    height: calc(90px + 4em);
    & img {
        width: 90px;
        height: 90px;
    }
}
.JPCDText {
    display: flex;
    flex-direction: column;
    row-gap: .4em;
    padding-left: 1em;
}
</style>