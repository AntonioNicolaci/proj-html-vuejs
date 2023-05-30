
<script>
export default {
    props: {
        team1: String,
        team2: String,
    }
}
</script>
<template>
    <div class="card">
        <img :src="`../../../public/img/${team1}`" alt="team1">
        <img src="../../../public/img/vs.png" alt="vs">
        <img :src="`../../../public/img/${team2}`" alt="team2">
    </div>
</template>
<style lang="scss" scoped>
    .card {
        background-color: #232a5c;
        display: flex;
        flex-direction: row;
    }
</style>