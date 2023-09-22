<script>
export default {

    name: 'AppHeader',
    data() {

        return {
            logo: '../assets/img/dc-logo.png',
            activeLink: 0,
            links: [
                {
                    nomeLink: 'characters'
                },

                {
                    nomeLink: 'comics'
                },

                {
                    nomeLink: 'movies'
                },

                {
                    nomeLink: 'tv'
                },

                {
                    nomeLink: 'games'
                },

                {
                    nomeLink: 'collectibles'
                },

                {
                    nomeLink: 'videos'
                },

                {
                    nomeLink: 'fans'
                },

                {
                    nomeLink: 'news'
                },

                {
                    nomeLink: 'shop'
                },
            ]

        }
    },
    components: {

    },
    methods: {
        changeActive(i) {
            this.activeLink = i
        },
    }

}

</script>

<template>
    <header id="app_header">
        <div class="container d-flex justify-content-between align-items-center ">
            <div class="logo-img">
                <a href="#"><img src="../assets/img/dc-logo.png" alt=""></a>
            </div>
            <ul class="list-unstyled d-flex gap-4">

                <li v-for="(link, i) in links">
                    <a href="#" @click="changeActive(i)" :class="(i == activeLink ? 'active' : '')">{{ link.nomeLink }}</a>
                </li>

            </ul>
        </div>
    </header>
</template>

<style lang="scss">
@use '../assets/scss/partials/variables' as *;

#app_header {
    padding: 1rem;
    background-color: $dc_white ;

    a {
        text-transform: uppercase;
        color: $dc_dark_black;

        &.active {
            padding-bottom: 2.5rem;
            color: $dc_primary;
            border-bottom: 10px solid;
        }
    }
}
</style>
