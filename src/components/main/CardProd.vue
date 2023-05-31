<script>
import { BIconStar, BIconStarFill } from 'bootstrap-icons-vue';
export default {
    props: {
        img: String,
        nameProd: String,
        price: Number,
        rating: Number,
    },
    components: {
        BIconStar,
        BIconStarFill,
    }
}
</script>
<template>
    <div class="CardDivProd">
        <img :src="`../../../public/img/${img}`" alt="img-T-Shirt">
        <div class="CardivProdBody">
            <span>{{ nameProd }}</span>
            <span>${{ price }}.00</span>
            <div class="DivStar">
                <template v-for="n in 5">
                    <BIconStarFill v-if="rating >= n" />
                    <BIconStar v-else />
                </template>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.CardDivProd {
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: #232a5c;

    & img {
        padding: .5em;
    }
}
.CardivProdBody {
        display: flex;
        flex-direction: column;
        align-items: center;
}
.DivStar {
    display: flex;
    flex-direction: row;
}
</style>