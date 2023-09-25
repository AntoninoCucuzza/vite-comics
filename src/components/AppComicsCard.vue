<script>
export default {
    name: 'AppComicsCard',
    setup() {
        return {}
    },
    props: ['thumb', 'series']
}
</script>
<template>
    <div class="col-2 flex-wrap">
        <div class="wapper">
            <img :src="thumb" alt="thumb" class="img-fluid w-100">
            <span class="text-white">{{ series }}</span>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.wapper {
    margin: 1rem 0;

    img {
        height: 275px;
        transition: all 0.5s;

        &:hover {
            scale: 1.2;
        }
    }
}
</style>