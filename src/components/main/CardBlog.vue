<script>
import ButtonApp from '../ButtonApp.vue';
export default {
    props:{
        img: String,
        text: String,
        writer: String,
        data: String,
        content: String,
        link: String,
    },
    components:{
        ButtonApp,
    }
}
</script>
<template>
    <div class="cardBlog">
        <img :src="`../../../public/img/${img}`" :alt="text">
        <div class="cardBlogText">
            <h4>{{ text }}</h4>
            <span>{{ writer }} | {{ data }}</span>
            <p>{{ content }}</p>
            <ButtonApp :text="'READ MORE'" :link="link" :classCSS=[] />
        </div>
    </div>
</template>
<style lang="scss" scoped>
    .cardBlog{
        width: calc(100% / 2 - 1em);
        height: fit-content;
        background-color: rgba(35, 42, 92, 0.7);
        display: flex;
        flex-direction: column;
        gap: 1em;
    }
    .cardBlogText {
        display: flex;
        flex-direction: column;
        row-gap: 1em;
        padding: 1.5em;
    }
    img {
        width: 100%;
        padding: .5em;
    }
</style>