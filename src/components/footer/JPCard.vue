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
    <div>
        <img :src="`../../../public/img/${logo}`" :alt="logo">
        <div>
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
<style lang="scss" scoped></style>