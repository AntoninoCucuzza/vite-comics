<script>
import AppMainJumbo from './AppMainJumbo.vue'
import AppComics from './AppComics.vue'
export default {

    name: 'AppMain',
    data() {
        return {

        }
    },
    components: {
        AppMainJumbo,
        AppComics
    }

}

</script>

<template>
    <AppMainJumbo />
    <AppComics />
    <main class="d-flex justify-content-between align-items-center ">
        <div class="container">
            <h1 class="text-white text-center"> (☞ﾟヮﾟ)☞ content here ☜(ﾟヮﾟ☜) </h1>
        </div>
    </main>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

main {

    background-color: $dc_main_dark;
}
</style>
