<script>
import CardProd from './CardProd.vue';
export default {
    data() {
        return {
            prodCard: [
                {
                    img: '01 (1).jpg',
                    nameProd: 'FROG T-SHIRT HERE',
                    price: 380.00,
                    rating: 5,
                },
                {
                    img: '02 (1).jpg',
                    nameProd: 'JOKER T-SHIRT HERE',
                    price: 380.00,
                    rating: 5,
                },
                {
                    img: '01 (1).jpg',
                    nameProd: 'GORILLAZ T-SHIRT HERE',
                    price: 380.00,
                    rating: 5,
                },
                {
                    img: '02 (1).jpg',
                    nameProd: 'ROBOTO T-SHIRT HERE',
                    price: 380.00,
                    rating: 5,
                },
            ]
        }
    },
    components: {
        CardProd,
    }
}
</script>
<template>
    <div id="CDDiv">
        <p>GAMER T-SHIRT'S</p>
        <h2>EXPLORE UOR PRODUCTS</h2>
        <div id="DivCardProd">
            <CardProd v-for="PC in prodCard" :img="PC.img" :nameProd="PC.nameProd" :price="PC.price" :rating="PC.rating"/>
        </div>
    </div>
</template>
<style lang="scss" scoped>
#CDDiv {
    display: flex;
    flex-direction: column;
    align-items: center;
    row-gap: 1em;
    & p{
        margin-top: 6em;
    }
}

#DivCardProd {
    display: flex;
    gap: 1em;
    padding-block: 1em 6em;
    border-bottom: 1px solid #444;
}
</style>