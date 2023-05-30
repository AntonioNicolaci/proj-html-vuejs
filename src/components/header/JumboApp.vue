<script>
import ButtonApp from '../ButtonApp.vue';
export default {
    components: {
        ButtonApp,
    }
}
</script>

<template>
    <div class="align-left">
        <h1>ONLINE GAME</h1>
        <h2>GENUINE MONEY TRANSACTION</h2>
        <p>Assertively Communicate An Expanded Array Of Mindshare Rather Than Diverse Technologies For Magnetic Applications Eamlessly Virtual Then Conveniently Monetize Synergistic Human Capital</p>
        <ButtonApp 
        :text="'ciao'"
        :link="'\#'"
        :classCSS="[]"/>
    </div>
</template>

<style lang="scss" scoped>
    div {
        display: flex;
        flex-direction: column;
        color: #fff;
        font-size: 1.7em;
        max-width: 50%;
        position: absolute;
        top: 50%;
    }
    h1{
        text-shadow: 3px 3px 5px red;
    }
</style>