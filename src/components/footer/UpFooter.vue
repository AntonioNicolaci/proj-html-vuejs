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
    <div>
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
<style lang="scss" scoped></style>