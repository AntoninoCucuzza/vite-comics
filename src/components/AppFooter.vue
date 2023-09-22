<script>
export default {

    name: 'AppFooter',
    data() {
        return {
            /* sconsiglio di aprire questi array */
            listComics: [
                {
                    nav: 'Characters'
                },

                {
                    nav: 'Comics'
                },

                {
                    nav: 'Movies'
                },

                {
                    nav: 'TV'
                },

                {
                    nav: 'Games'
                },

                {
                    nav: 'Videos'
                },

                {
                    nav: 'News'
                }

            ],

            listShop: [
                {
                    nav: 'Shop DC'
                },

                {
                    nav: 'Shop DC Collectibles'
                }

            ],

            listDc: [
                {
                    nav: 'Terms Of Use'
                },

                {
                    nav: 'Privacy Policy (New)'
                },

                {
                    nav: 'Ad Choices'
                },

                {
                    nav: 'Advertising'
                },

                {
                    nav: 'Jobs'
                },

                {
                    nav: 'Subscription'
                },

                {
                    nav: 'Talent Workshop'
                },

                {
                    nav: 'CPSC Certificates'
                },

                {
                    nav: 'Ratings'
                },

                {
                    nav: 'Shop Help'
                },

                {
                    nav: 'Contact Us'
                }

            ],

            listSites: [
                {
                    nav: 'DC'
                },

                {
                    nav: 'MAD Magazine'
                },

                {
                    nav: 'DC Kids'
                },

                {
                    nav: 'DC Universe'
                },

                {
                    nav: 'DC Power Visa'
                }

            ]
        }
    },


}

</script>

<template>
    <footer class=" d-flex ">
        <div class="container">
            <div class="row  ">
                <div class="col-2 help">
                    <h3>dc comics</h3>
                    <ul class="list-unstyled">
                        <li v-for="link in listComics">
                            <a href="#">{{ link.nav }}</a>
                        </li>
                    </ul>

                    <h3>shop</h3>
                    <ul class="list-unstyled">
                        <li v-for="link in listShop">
                            <a href="#">{{ link.nav }}</a>
                        </li>
                    </ul>
                </div>

                <div class="col-2 help">
                    <h3>DC</h3>
                    <ul class="list-unstyled">
                        <li v-for="link in listDc">
                            <a href="#">{{ link.nav }}</a>
                        </li>
                    </ul>
                </div>

                <div class="col-2 help ">
                    <h3>sites</h3>
                    <ul class="list-unstyled">
                        <li v-for="link in listSites">
                            <a href="#">{{ link.nav }}</a>
                        </li>
                    </ul>
                </div>
                <div class="col-6 bg_logo">
                </div>
            </div>

        </div>

    </footer>
</template>
 
<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

footer {
    color: $dc_white;
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    background-repeat: no-repeat;


    h3 {
        text-transform: uppercase;
    }

    a {
        color: $dc_dark_gray;
    }

    .help {
        padding: 2rem 0;
    }

    .bg_logo {
        background-image: url('../assets/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: center;
    }
}
</style>
