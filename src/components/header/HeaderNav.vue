<script>
export default {
    name: "Nav",
    data() {
        return {
            links: [
                {
                    link: "Characters",
                    href: "#",
                },
                {
                    link: "Comics",
                    href: "#",
                },
                {
                    link: "Movies",
                    href: "#",
                },
                {
                    link: "Tv",
                    href: "#",
                },
                {
                    link: "Games",
                    href: "#",
                },
                {
                    link: "Collectibles",
                    href: "#",
                },
                {
                    link: "Videos",
                    href: "#",
                },
                {
                    link: "Fans",
                    href: "#",
                },
                {
                    link: "News",
                    href: "#",
                },
                {
                    link: "Shop",
                    href: "#",
                },
            ],
        };
    },
};
</script>

<template>
    <nav>
        <a v-for="link in links" :href="link.href">{{ link.link.toUpperCase() }}</a>
    </nav>
</template>

<style lang="scss">
nav {
    display: flex;
    flex-wrap: wrap;
    gap: 35px;

    a {
        text-decoration: none;
        color: #464646;
        font-weight: bold;

        &:hover {
            color: #0282f9;
        }
    }
}
</style>
