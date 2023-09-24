<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue'
import AppFooterTop from './components/AppFooterTop.vue'
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
        AppFooterTop,
        AppFooter,
        AppFooterBot
    }

}

</script>

<template>
    <AppHeader />
    <AppMain />
    <AppFooterTop />
    <AppFooter />
    <AppFooterBot />
</template>

<style lang="scss" scoped></style>
