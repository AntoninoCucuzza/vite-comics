<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue'
import AppFooterTope from './components/AppFooterTope.vue'
import AppFooterBot from './components/AppFooterBot.vue'



export default {
    name: 'App',
    data() {
        return {
            message: 'ello'
        }
    },
    components: {
        AppHeader,
        AppMain,
        AppFooterTope,
        AppFooter,
        AppFooterBot
    }

}

</script>

<template>
    <AppHeader />
    <AppMain />
    <AppFooterTope />
    <AppFooter />
    <AppFooterBot />
</template>

<style lang="scss" scoped></style>
