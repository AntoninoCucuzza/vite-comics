<script>
export default {

    name: 'AppFooterTop',
    data() {
        return {
            listInfo: [
                {
                    img: './src/assets/img/buy-comics-digital-comics.png',
                    text: 'digital comics'
                },
                {
                    img: './src/assets/img/buy-comics-merchandise.png',
                    text: 'dc merchandise'
                },
                {
                    img: './src/assets/img/buy-comics-subscriptions.png',
                    text: 'subscription'
                },
                {
                    img: './src/assets/img/buy-comics-shop-locator.png',
                    text: 'comic shop locator'
                },
                {
                    img: "./src/assets/img/buy-dc-power-visa.svg",
                    text: 'dc power visa'
                },
            ]
        }
    },


}

</script>

<template>
    <footer id="top_footer">
        <div class="container">
            <div class="row">
                <a href="#" v-for="info in listInfo" class="col d-flex justify-content-center align-items-center gap-2">
                    <img class="w-25" :src="info.img" alt="">
                    {{ info.text }}
                </a>
            </div>
        </div>

    </footer>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#top_footer {
    background-color: $dc_primary;
    padding: 3rem;

    a {
        color: white;

        img {
            height: 70px;
            object-fit: scale-down;
        }
    }
}
</style>
