<script>
export default {

    name: 'AppFooterBot',
    data() {
        return {
            socials: [
                {
                    img: './src/assets/img/footer-facebook.png',
                    name: 'facebook',
                    link: 'https://www.facebook.com/?locale=it_IT',

                },

                {
                    img: './src/assets/img/footer-twitter.png',
                    name: 'twitter',
                    link: 'https://twitter.com/?lang=it',

                },

                {
                    img: './src/assets/img/footer-youtube.png',
                    name: 'youtube',
                    link: 'https://www.youtube.com',

                },

                {
                    img: './src/assets/img/footer-pinterest.png',
                    name: 'pinterest',
                    link: 'https://www.pinterest.it',

                },

                {
                    img: './src/assets/img/footer-periscope.png',
                    name: 'periscope',
                    link: 'https://www.pscp.tv',

                },

            ]
        }
    },
}

</script>

<template>
    <div id="footer_bot">
        <div class="container">
            <div class="row">
                <div class="d-flex justify-content-between align-items-center">
                    <div class="left d-flex ">
                        <a id="sign-in" href="#">
                            Sign-up now!
                        </a>
                    </div>
                    <div class="right d-flex">
                        <a id="Follow-us" href="#">
                            <h4 class="text-uppercase m-0">follow us</h4>
                        </a>
                        <a v-for="social in socials" target="blank" :href="social.link" class="ms-4">
                            <img class="socials" :src="social.img" alt="">
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#footer_bot {
    padding: 2.5rem;
    background-color: $dc_dark_black;

    .left {
        #sign-in {
            color: $dc_white;
            text-transform: uppercase;
            border: 3px solid $dc_primary;
            border-radius: 0;
            padding: 0.7rem 0.8rem;
            font-weight: bold;
            transition: all 0.3s;

            &:hover {
                background-color: $dc_primary;
                color: $dc_main_dark ;
            }
        }
    }

    .right {
        #Follow-us {
            color: $dc_primary;
        }

        .socials {
            border-radius: 50%;
            transition: background-color 0.2s;

            &:hover {
                background-color: $dc_primary;
                box-shadow: 0px 0px 15px 2px;
            }
        }
    }
}
</style>
