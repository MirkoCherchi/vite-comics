<script>
import Products from './Products.vue';
export default {
    name: 'MainTop',
    components: {
        Products
    },

}

</script>

<template>
    <div class="main-top">
        <div class="container">
            <h3>Current series</h3>
            <Products />
            <div class="button-main">
                <button>load more</button>
            </div>


        </div>
    </div>
</template>

<style scoped lang="scss">
.main-top {
    background-color: #1c1c1c;

    .container {
        position: relative;

        .button-main {
            display: flex;
            justify-content: center;
            align-items: center;
            padding-bottom: 20px;

            button {
                all: unset;
                background-color: #0282F9;
                text-transform: uppercase;
                color: #fff;
                padding: 10px 70px;
                font-size: 1rem;
            }
        }
    }

    h3 {
        color: white;
        text-transform: uppercase;
        padding: 10px 20px;
        position: absolute;
        top: 0;
        left: 0;
        transform: translate(15px, -50%);
        font-size: 1.5rem;
        z-index: 1;
        background-color: #0282F9;
    }
}
</style>
