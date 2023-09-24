<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue'
import AppFooterTop from './components/AppFooterTop.vue'


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
        AppFooter,
        AppFooterTop,
    }

}

</script>

<template>
    <AppHeader />
    <AppMain />
    <AppFooterTop />
    <AppFooter />
</template>

<style lang="scss" scoped></style>
