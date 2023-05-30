<script>
import { BIconGeoAltFill, BIconTelephoneFill, BIconMessenger, BIconTwitter, BIconVimeo, BIconSkype, BIconWifi } from 'bootstrap-icons-vue';
import ButtonApp from '../ButtonApp.vue';

export default {

    data() {
        return {
            buttonUpBar: [
                {
                    text: "HOME",
                    link: "#",
                    classCSS: [
                        "whiteBTN",
                    ]
                },
                {
                    text: "FEATURES +",
                    link: "#",
                    classCSS: [
                        "whiteBTN",
                    ]
                },
                {
                    text: "ACHIEVEMENT",
                    link: "#",
                    classCSS: [
                        "whiteBTN",
                    ]
                },
                {
                    text: "BLOG +",
                    link: "#",
                    classCSS: [
                        "whiteBTN",
                    ]
                },
                {
                    text: "CONTACT",
                    link: "#",
                    classCSS: [
                        "whiteBTN",
                    ]
                },
            ],
            buttondownBar: [
            {
                    text: "LOG IN",
                    link: "#",
                    classCSS: [
                    ]
                },
                {
                    text: "SING IN",
                    link: "#",
                    classCSS: [
                    ]
                },
            ]
        }
    },

    components: {
        BIconGeoAltFill,
        BIconTelephoneFill,
        BIconMessenger,
        BIconTwitter,
        BIconVimeo,
        BIconSkype,
        BIconWifi,
        ButtonApp,
    }
}
</script>

<template>
    <nav>
        <div id="upBar">
            <div id="number">
                <BIconTelephoneFill />
                +800-123-4567-6587
            </div>
            <div id="position">
                <BIconGeoAltFill />
                Beverley, New York 224 USA
            </div>
            <div id="social">
                <BIconMessenger />
                <BIconTwitter />
                <BIconVimeo />
                <BIconSkype />
                <BIconWifi />
            </div>
        </div>
        <div id="downBar">
            <img src="../../../public/img/logo.png" alt="logo">
            <div id="btnW">
                <ButtonApp v-for="btn in buttonUpBar"
                    :text="btn.text"
                    :link="btn.link"
                    :classBTN="btn.classCSS"
                />    
            </div>
            <div id="btnC">
                <ButtonApp v-for="btn in buttondownBar"
                    :text="btn.text"
                    :link="btn.link"
                    :classBTN="btn.classCSS"
                />    
            </div>
        </div>
        <div></div>
    </nav>
</template>

<style lang="scss" scoped>
nav {
    background-color: rgba(35, 42, 92, 0.8)
}

#upBar {
    display: flex;
    justify-content: space-between;
    color: #fff;
    border-bottom: 1px solid #fff;
}

#number,
#position,
#social {
    height: 3em;
    display: flex;
    align-items: center;
}

#number {
    margin-left: 2em;
    border-inline: 1px solid #fff;
}

#position {
    width: 50%;
    align-self: start;
}

#social {
    gap: 1em;

    &:only-child {
        border-right: 1px solid #fff;
    }
}

#downBar{
    display: flex;
    align-items: center;
}

#btnW{
    display: flex;
    gap: 2em;
}
</style>