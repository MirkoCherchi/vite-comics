<script>
import Header from './components/header/HeaderComponents.vue';
import Main from './components/main/MainComponents.vue';
export default {
    name: "app",
    components: {
        Header,
        Main,
    },
};
</script>

<template>
    <Header />
    <Main />
</template>

<style lang="scss">
@use "./styles/cont.scss" as *;
</style>
