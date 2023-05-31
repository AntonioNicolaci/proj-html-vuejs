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
    <a :href="link" :class="classBTN">{{ text }}</a>
</template>

<style lang="scss" scoped>
a {
    text-decoration: none;
    padding: 1em;
}

.whiteBTN {
    font-weight: bold;
    color: #fff;
}
.whiteBG {
    background-color: #fff;
}
.redBG{
    background-color: #ff0052;
}
.whiteColor{
    color: #fff;
}
.redColor {
    color: #ff0052;
}
.redBorder{
    border-bottom: 2px solid #ff0052;
    border-right: 2px solid #ff0052;
}
.whiteBorder{
    border-bottom: 2px solid #fff;
    border-right: 2px solid #fff;
}
</style>