<script>
import AppJumbotron from './AppJumbotron.vue'
import AppComicsCard from './AppComicsCard.vue'
import comicss from '../comicss.js'
export default {

    name: 'AppMain',
    data() {
        return {
            comicss
        }
    },
    components: {
        AppJumbotron,
        AppComicsCard,
    }

}

</script>

<template>
    <AppJumbotron />
    <main class="d-flex justify-content-between align-items-center ">
        <div class="container">
            <div class="row">
                <AppComicsCard v-for="product in comicss" :thumb="product.thumb" :series="product.series" />
            </div>
            <div class="d-flex justify-content-center align-items-center">
                <a href="#">load more</a>
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

main {
    padding: 2rem;
    padding-top: 4rem;
    background-color: $dc_main_dark;

    a {
        text-transform: uppercase;
        font-weight: bold;
        color: white;
        background-color: $dc_primary;
        border: 2px solid $dc_primary;
        padding: 0.5rem 2rem;
    }
}
</style>
