<script>
import MainTop from '../main/MainTop.vue';
import MainBottom from '../main/MainBottom.vue';
export default {
    name: 'Main',
    components: {
        MainTop,
        MainBottom,
    }

}

</script>

<template>
    <main>
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
