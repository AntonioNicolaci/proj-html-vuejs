<script>
import { BIconGeoAlt, BIconEnvelope} from 'bootstrap-icons-vue'
export default {
    components: {
        BIconGeoAlt,
        BIconEnvelope,
    }
}
</script>
<template>
    <div id="UFDiv">
        <div>
            <img src="../../../public/img/01 (4).png" alt="">
            <span>Phone Number: +88012 3454 6778 912</span>
        </div>
        <div>
            <BIconEnvelope />
            <span>email: youremail@gmail.com</span>
        </div>
        <div>
            <BIconGeoAlt />
            <span>Address: 30 North West New York 240</span>
        </div>
    </div>
</template>
<style lang="scss" scoped>
#UFDiv{
    display: flex;
    align-items: center;
    & div {
        display: flex;
        align-items: center;
        padding: 2em;
        border-inline: 1px solid rgba(100, 100, 100, 0.5);
        height: 6em;

        & svg {
            color: #ff0052;
        }
    }
}
</style>