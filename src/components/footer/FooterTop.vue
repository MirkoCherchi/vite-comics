<script>
export default {
    data() {
        return {
            links: [
                {
                    title: "DC Comics",
                    items: [
                        "Characters",
                        "Comics",
                        "Movies",
                        "TV",
                        "Games",
                        "Videos",
                        "News",
                    ],
                },
                {
                    title: "Shop",
                    items: ["Shop DC", "Shop DC Collectibles"],
                },
                {
                    title: "DC",
                    items: [
                        "Terms Of Use",
                        "Privacy Policy (New)",
                        "Ad Choices",
                        "Advertising",
                        "Jobs",
                        "Subscriptions",
                        "Talent Workshops",
                        "CPSC Certificates",
                        "Ratings",
                        "Shop Help",
                        "Contact Us",
                    ],
                },
                {
                    title: "Sites",
                    items: [
                        "DC",
                        "MAD Magazine",
                        "DC Kids",
                        "DC Universe",
                        "DC Power Visa",
                    ],
                },
            ],
        };
    },
};
</script>

<template>
    <div class="backimage">
        <div class="container">
            <div class="links">
                <div class="left">
                    <div v-for="(link, index) in links" v-show="index <= 1">
                        <h3>{{ link.title }}</h3>
                        <ul>
                            <li v-for="item in link.items">
                                <a href="#"> {{ item }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="right">
                    <div v-for="(link, index) in links" v-show="index >= 2">
                        <h3>{{ link.title }}</h3>
                        <ul>
                            <li v-for="item in link.items">
                                <a href="#"> {{ item }}</a>
                            </li>
                        </ul>
                    </div>
                </div>

            </div>
            <div class="back-logo"></div>


        </div>
    </div>
</template>

<style lang="scss" scoped>
.backimage {
    background-image: url(../../../public/img/footer-bg.jpg);
    background-size: cover;
    background-repeat: no-repeat;
}

.back-logo {
    background-image: url(../../../public/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    width: 100%;
    background-position: right;
}

.links {
    display: flex;
    padding-top: 35px;
    padding-bottom: 55px;
    gap: 30px;
}

.container {
    display: flex;

    .right {
        display: flex;
        gap: 30px;
    }

    .left {
        display: flex;
        flex-direction: column;
        gap: 25px;
    }

    div {
        h3 {
            color: white;
            padding-bottom: 20px;
        }

        ul {
            list-style-type: none;
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            gap: 10px;

            li {
                font-size: 14px;
                font-family: "Open Sans", sans-serif;
                color: #959595;
                margin-right: 55px;
                width: 100%;

                a {
                    text-decoration: none;
                    color: gray;
                }
            }
        }
    }
}
</style>
