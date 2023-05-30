<script>
import TodayCard from './TodayCard.vue';
import ButtonApp from '../ButtonApp.vue';
import TodaysDiv from './TodaysDiv.vue';
import ProTeam from './ProTeam.vue';
import AllMatches from './AllMatches.vue';
export default {
    components: {
    TodayCard,
    ButtonApp,
    TodaysDiv,
    ProTeam,
    AllMatches,
}
}
</script>

<template>
    <main>
        <div class="mainDivCol align">
            <TodaysDiv />
        </div>
        <div class="mainDivRow align">
            <ProTeam />
        </div>
        <div class="mainDiv" id="allMatch">
            <AllMatches />
        </div>
        <!-- <div class="mainDiv">
            <MeetSquad />
        </div>
        <div class="mainDiv">
            <JoinGame />
        </div>
        <div class="mainDiv">
            <CheckLive />
        </div>
        <div class="mainDiv">
            <Products />
        </div>
        <div class="mainDiv">
            <BecomePartner />
        </div>
        <div class="mainDiv">
            <Blog />
        </div>
        <div class="mainDiv">
            <Testimonial />
        </div> -->
    </main>
</template>

<style lang="scss" scoped>
main {
    background-color: #131661;
}

.mainDivCol {
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    max-width: 100%;
}
.mainDivRow{
    display: flex;
    justify-content: center;
    align-items: center;
    max-width: 100%;
}
#allMatch {
    background: url('../../../public/img/bg\ \(1\).jpg');
    height: 1382px;
}
</style>