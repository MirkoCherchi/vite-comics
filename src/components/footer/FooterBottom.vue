<script>
export default {
    data() {
        return {
            socialIcons: [
                {
                    name: "Facebook",
                    img: '/img/footer-facebook.png'
                },
                {
                    name: "Twitter",
                    img: '/img/footer-twitter.png'
                },
                {
                    name: "YouTube",
                    img: '/img/footer-youtube.png'
                },
                {
                    name: "Pinterest",
                    img: '/img/footer-pinterest.png'
                },
                {
                    name: "Periscope",
                    img: '/img/footer-periscope.png'
                },
            ]
        }
    }
};
</script>



<template>
    <div class="cont-foot-bottom">
        <div class="container">
            <div class="foot-bottom-left"><button>Sign-up now!</button></div>
            <div class="foot-bottom-right">
                <h4>Follow Us</h4>
                <ul>
                    <li v-for="social in socialIcons"><img :src="social.img" :alt="social.name"></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.cont-foot-bottom {
    background-color: #303030;

    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 30px 0;
    }

    button {
        all: unset;
        border: 2px solid #0282f9;
        padding: 15px;
        text-transform: uppercase;
        color: #fff;
        cursor: pointer;
    }

    .foot-bottom-right {

        display: flex;
        justify-content: center;
        align-items: center;

        h4 {
            color: #0282f9;
            padding-right: 30px;
            font-size: 24px;
            text-transform: uppercase;
        }

        ul {
            display: flex;
            justify-content: center;
            align-items: center;
            list-style: none;
            gap: 20px;
        }

        img {
            cursor: pointer;
        }

    }

}
</style>
