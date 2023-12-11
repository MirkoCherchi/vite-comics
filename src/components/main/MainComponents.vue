<script>
import MainTop from '../main/MainTop.vue';
import MainBottom from '../main/MainBottom.vue';
import MainJumbotron from './MainJumbotron.vue';
export default {
    name: 'Main',
    components: {
        MainTop,
        MainBottom,
        MainJumbotron,

    }

}

</script>

<template>
    <main>
        <MainJumbotron />
        <MainTop />
        <MainBottom />

    </main>
</template>

<style lang="scss">
main {
    display: flex;
    flex-direction: column;
}
</style>
