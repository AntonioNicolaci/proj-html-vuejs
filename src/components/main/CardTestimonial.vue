<script>
import {BIconStar} from 'bootstrap-icons-vue';
export default {
    data() {
        return {
            StarRating: Math.floor(this.rating),
        }
    },
    props: {
        nameTes: String,
        imgTes: String,
        work: String,
        logo: String,
        content: String,
        rating: Number,
    },
    components: {
        BIconStar,
    }
}
</script>
<template>
    <div class="CTDiv">
        <div class="CTDTes">
            <div class="CTDTPers">
                <img :src="`../../../public/img/${imgTes}`" :alt="nameTes">
                <div>
                    <span class="nameTes">{{ nameTes }}</span>
                    <span>{{ work }}</span>
                </div>
            </div>
            <img :src="`../../../public/img/${logo}`" :alt="logo">
        </div>
        <div class="CTDText">
            <p>{{ content }}</p>
            <div class="DivstarDiv">
                <template  v-for="n in 10">
                    <div v-if="StarRating >= n" class="starDiv">
                        <BIconStar />
                    </div>
                </template>
                <span>{{ rating }}</span>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.CTDiv {
    display: flex;
    flex-direction: column;
    padding: 1em;
    background-color: #232a5c;

    & p {
        color: #fff;
    }
}

.CTDTes {
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-bottom: 1px solid #555;
    padding: 1em;
}
.CTDTPers{
    display: flex;
    align-items: center;

    & div {
        display: flex;
        flex-direction: column;
        row-gap: 1em;
    }

    & img {
        border-radius: 50%;
        padding-right: 1em;
    }
}
.nameTes{
    font-weight: bold;
}

.CTDText {
    display: flex;
    flex-direction: column;
    gap: 1em;
    padding-block: 1em;
}
.DivstarDiv {
    display: flex;
    align-items: center;
    gap: .5em;
}
.starDiv{
    background-color: #00b67a;
    border-radius: 5px;
    width: 2em;
    height: 2em;
    display: flex;
    align-items: center;
    justify-content: center;
    
    & span {
        color: #00b67a;
    }
}
</style>