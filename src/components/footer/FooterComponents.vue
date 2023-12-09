<script>
import FooterTop from "./FooterTop.vue";
import FooterBottom from "./FooterBottom.vue";
export default {
    components: {
        FooterTop,
        FooterBottom,
    },
};
</script>

<template>
    <footer>
        <FooterTop />
        <FooterBottom />
    </footer>
</template>

<style lang="scss">
.footer-flex {
    display: flex;
    flex-direction: column;
}
</style>
