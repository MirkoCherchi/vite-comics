<script>
import Nav from "../header/HeaderNav.vue";
import LogoHeader from "../header/HeaderLogo.vue";
export default {
    name: "Header",
    components: {
        Nav,
        LogoHeader,
    },
};
</script>

<template>
    <div class="container">
        <header>
            <LogoHeader />
            <Nav />
        </header>
    </div>
</template>

<style lang="scss">
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 0;
}
</style>
