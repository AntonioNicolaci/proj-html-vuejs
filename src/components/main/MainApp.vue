<script>
import TodayCard from './TodayCard.vue';
import ButtonApp from '../ButtonApp.vue';
import TodaysDiv from './TodaysDiv.vue';
import ProTeam from './ProTeam.vue';
import AllMatches from './AllMatches.vue';
import MeetSquad from './MeetSquad.vue';
import JoinGame from './JoinGame.vue';
import CheckLive from './CheckLive.vue';
import Products from './Products.vue';
import BecomePartner from './BecomePartner.vue';
import Blog from './Blog.vue';
import Testimonial from './Testimonial.vue';
export default {
    components: {
        TodayCard,
        ButtonApp,
        TodaysDiv,
        ProTeam,
        AllMatches,
        MeetSquad,
        JoinGame,
        CheckLive,
        Products,
        BecomePartner,
        Blog,
        Testimonial,
    }
}
</script>

<template>
    <main>
        <TodaysDiv />
        <div class="align">
            <ProTeam />
        </div>
        <div id="allmatch">
            <AllMatches />
        </div>
        <MeetSquad />
        <JoinGame />
        <div id="checklive">
            <CheckLive />
        </div>
        <Products />
        <BecomePartner />
        <div id="blog">
            <Blog />
        </div>
        <div id="testimonial">
            <Testimonial />
        </div>
    </main>
</template>

<style lang="scss" scoped>
main {
    background-color: #131661;
    color: #fff;
}

.mainDivCol {
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    max-width: 100%;
}

.mainDivRow {
    display: flex;
    justify-content: center;
    align-items: center;
    max-width: 100%;
}

#allmatch {
    background: url('../../../public/img/bg\ \(1\).jpg');
    height: 1382px;
}
#checklive{
    background-image: url('../../../public/img/bg\ \(3\).jpg');
}
#blog{
    background-image: url('../../../public/img/bg\ \(2\).jpg');
}
#testimonial {
    background: url('../../../public/img/bg.png') ;
    height: 675px;
}
</style>