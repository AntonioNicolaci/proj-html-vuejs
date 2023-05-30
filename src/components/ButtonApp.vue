<script>
export default {
    props: {
        text: String,
        link: String,
        classBTN: Array,
    }
}
</script>

<template>
    <a :href="link"
    :class="classBTN"
    >{{ text }}</a>
</template>

<style lang="scss" scoped>
a{
    text-decoration: none;
}
.whiteBTN{
    color: #fff;
    font-weight: bold;
}
</style>