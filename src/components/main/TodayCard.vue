
<script>
export default {
    props: {
        team1: String,
        team2: String,
    }
}
</script>
<template>
    <div>
        <div class="card">
            <img :src="`../../../public/img/${team1}`" alt="team1">
            <img src="../../../public/img/vs.png" alt="vs" class="vs">
            <img :src="`../../../public/img/${team2}`" alt="team2">
        </div>
        <div class="divLL">
            <div class="lungo">
                <div class="largo"></div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.card {
    background-color: #232a5c;
    display: flex;
    align-items: center;
    padding: 3em 2em;
    border-radius: 8px;
    gap: 1em;
    max-height: 12em;
}
</style>