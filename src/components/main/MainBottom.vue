<script>
export default {
    name: 'Card',
    data() {
        return {
            cards: [
                {
                    card: '/img/buy-comics-digital-comics.png',
                    description: 'Digital Comics'
                },
                {
                    card: '/img/buy-comics-merchandise.png',
                    description: 'Dc merchandise'
                },
                {
                    card: '/img/buy-comics-subscriptions.png',
                    description: 'Subscription'
                },
                {
                    card: '/img/buy-comics-shop-locator.png',
                    description: 'Comic shop locator'
                },
                {
                    card: '/img/buy-dc-power-visa.svg',
                    description: 'dc power visa'
                },
            ]
        }
    }

}

</script>

<template>
    <div class="cards">
        <div class="container">
            <div class="list-card">
                <a v-for="card in cards" href="#"><img :src="card.card" alt="">
                    <p>{{ card.description.toLocaleUpperCase() }}</p>
                </a>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
.cards {
    background-color: #0282f9;

    img {
        width: 45px;
        height: 45px;
    }

    .list-card {
        display: flex;
        align-items: center;
        flex-wrap: nowrap;
        justify-content: space-between;
        padding: 45px;
        gap: 60px;
        padding-left: 40px;

    }

    a {
        display: flex;
        align-items: center;
        height: 100%;
        gap: 15px;
        text-decoration: none;
        font-size: 1rem;
        color: #fff;

    }


}
</style>
