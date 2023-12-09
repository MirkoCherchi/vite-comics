<script>
import Header from "./components/header/HeaderComponents.vue";
import Main from "./components/main/MainComponents.vue";
import Footer from "./components/footer/FooterComponents.vue";
export default {
    name: "app",
    components: {
        Header,
        Main,
        Footer,
    },
};
</script>

<template>
    <Header />
    <Main />
    <Footer />
</template>

<style lang="scss">
@use "./styles/cont.scss" as *;
</style>
