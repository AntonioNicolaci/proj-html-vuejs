<script>
import CardTestimonial from './CardTestimonial.vue';
export default {
    data() {
        return {
            tesCard: [
                {
                    nameTes: 'MADLEY PONDOR',
                    imgTes: '01 (2).jpg',
                    work: 'UI Designer',
                    logo: '08.png',
                    content: 'Edgeing nterfaces fnergstca pagiarize teams anbudng paradgms rapidiousl buildcaboration anden deassharing viaing nad bleeding whereas goingi forward process and monetze',
                    rating: 5.28
                },
                {
                    nameTes: 'OLIVER BEDDOWS',
                    imgTes: '01 (2).jpg',
                    work: 'UI Designer',
                    logo: '06.png',
                    content: 'Rapidious buildcaboration anden deas sharing viaing and beedng edgeing nterfaces fnergstcia plagiarize teams anbuding paradgm whereas goingi forward process and monetze',
                    rating: 5.28
                },
            ]
        }
    },
    components: {
        CardTestimonial,
    }
}
</script>
<template>
    <div id="TCard">
        <p>UOR RECENT NEWS</p>
        <h2>OUR MOST POPULAR TESTIMONIAL POSTS</h2>
        <div id="CDDiv" class="align">
            <CardTestimonial v-for="TC in tesCard" :nameTes="TC.nameTes" :imgTes="TC.imgTes" :work="TC.work" :logo="TC.logo"
                :content="TC.content" :rating="TC.rating" />
        </div>
    </div>
</template>
<style lang="scss" scoped>
#TCard {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 1em;
    padding-block: 6em;
}

#CDDiv {
    display: flex;
    gap: 1em;
    padding-top: 1em;
}
</style>