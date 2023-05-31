<script>
import CardBlog from './CardBlog.vue';
export default {
    data() {
        return {
            blogCard: [
                {
                    img:'01 (3).jpg',
                    text:'DISTINCTIVE REDEFINE RESOURCE MAXIMIZING FOR',
                    writer:'Admin',
                    data:'01 Januari 2022',
                    content:'Uniquely conceptuaze visiaonary process ariwith tactical ramatica centered qualitys vectoris with outofthbox scenario is ompelling uthoritatively generate front-end niches after one',
                    link:'#'
                },
                {
                    img:'05.jpg',
                    text:'REDEFINE RESOURCE MAXIMIZING FOR DISTINCTIVE',
                    writer:'Admin',
                    data:'01 Januari 2022',
                    content:'Uniquely conceptuaze visiaonary process ariwith tactical ramatica centered qualitys vectoris with outofthbox scenario is ompelling uthoritatively generate front-end niches after one',
                    link:'#'
                },
            ]
        }
    },
    components: {
        CardBlog,
    }
}
</script>
<template>
    <div id="BDiv">
        <p>OUR RECENT NEWS</p>
        <h2>OUR MOST POPULAR BLOCK POSTS</h2>
        <div id="BDDivCard" class="align">
            <CardBlog v-for="BC in blogCard" :img="BC.img" :text="BC.text" :writer="BC.writer" :data="BC.data" :content="BC.content" :link="BC.link"/>
        </div>
    </div>
</template>
<style lang="scss" scoped>
    #BDiv {
        display: flex;
        flex-direction: column;
        align-items: center;
        margin-top: 6em;
        row-gap: 1em;
        padding-block: 6em;
    }
    #BDDivCard {
        display: flex;
        gap: 1em;
        padding-top: 1em
    }
</style>