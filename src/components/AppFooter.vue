<script>
export default {
    name: "AppFooter",
    data() {
        return {
            dcComics: ["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"],
            shop: ["Shop DC", "Shop DC Collectibles"],
            dc: ["Terms Of Use", "Privacy Policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help", "Contact us"],
            sites: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],


            followInfo: [
                {
                    img: '../assets/img/footer-facebook.png',
                    href: '##'
                },
                {
                    img: '../assets/img/footer-twitter.png',
                    href: '##'
                },
                {
                    img: '../assets/img/footer-youtube.png',
                    href: '##'
                },
                {
                    img: '../assets/img/footer-pinterest.png',
                    href: '##'
                },
                {
                    img: '../assets/img/footer-periscope.png',
                    href: '##'
                }
            ]
        }
    }
}
</script>

<template>
    <footer id="site_footer">

        <div class="footer_info">

            <div class="container-info w-75 h-100  m-auto d-flex ">
                <div class="container d-flex align-items-center">
                    <div class="col-2">
                        <h3>DC COMICS</h3>
                        <ul>
                            <li v-for="item in dcComics">{{ item }}</li>
                        </ul>

                        <h3>SHOPS</h3>
                        <ul>
                            <li v-for="item in shop">{{ item }}</li>
                        </ul>
                    </div>
                    <div class="col-2">
                        <h3>DC</h3>
                        <ul>
                            <li v-for="item in dc">{{ item }}</li>
                        </ul>
                    </div>
                    <div class="col-2 height_68">
                        <h3>SITES</h3>
                        <ul>
                            <li v-for="item in sites">{{ item }}</li>
                        </ul>
                    </div>
                    <div class="col-6 logo"></div>
                </div>

            </div>

        </div>

        <div class="footer_social">
            <div class="container d-flex justify-content-between h-100">

                <div class=" d-flex align-items-center">
                    <a href="##">
                        <button class="btn btn-outline-primary text-uppercase text-white rounded-0 fs-5">
                            sign-up now!
                        </button>
                    </a>
                </div>

                <div class=" d-flex align-items-center gap-4">
                    <h5 class="m-0">FOLLOW US</h5>
                    <a v-for="icons in followInfo" href="followInfo.href">
                        <img :src="followInfo.img" alt="">
                    </a>
                </div>


            </div>
        </div>

    </footer>
</template>


<style lang="scss" scoped>
@use '../assets/scss/Partials/variables' as *;

.site_footer {
    height: 750px;
}

.footer_info {
    background-image: url("../assets/img/footer-bg.jpg");
    height: 600px;
    background-size: cover;


    & li {
        color: $dc_light_grey;
        list-style-type: none;
        font-size: 20px;
    }

    & ul {
        padding: 0
    }

    & h3 {
        color: $dc_white;
    }
}

.footer_social {
    height: 150px;
    background-color: $dc_dark_grey;

    & h5 {
        color: $dc_primary;
    }


}

.height_68 {
    height: 65%;
}

.logo {
    background-image: url("../assets/img/dc-logo-bg.png");
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    height: 100%;

}
</style>