<template>
    <footer class="debug">
        <div class="top_footer">
            <div class="container">
                <ul>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                            <div class="text">digital comics</div>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-merchandise.png" alt="">
                            <div class="text">dc merchandise</div>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                            <div class="text">subscription</div>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                            <div class="text">comic shop locator</div>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                            <div class="text">dc power visa</div>
                        </a>
                    </li>
                </ul>
            </div>
        </div>

        <div class="main_footer">
            <div class="container">

                <nav class="footer_nav">
                    <div class="ul_col one">
                        <ul id="dc_comics">
                            <li><a href="#">Dc Comics</a></li>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>

                        <ul id="shop">
                            <li><a href="#">Shop</a></li>
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Shop DC Collectibles</a></li>
                        </ul>
                    </div>

                    <div class="ul_col two">
                        <ul id="dc">
                            <li><a href="#">Dc</a></li>
                            <li><a href="#">Terme Of Use</a></li>
                            <li><a href="#">Privacy policy (New)</a></li>
                            <li><a href="#">Ad Choices</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Subscriptions</a></li>
                            <li><a href="#">Talent Workshops</a></li>
                            <li><a href="#">CPSC Certificates</a></li>
                            <li><a href="#">Rating</a></li>
                            <li><a href="#">Shop Help</a></li>
                            <li><a href="#">Contact Us</a></li>
                        </ul>
                    </div>

                    <div class="ul_col three">
                        <ul id="sites">
                            <li><a href="#">Sites</a></li>
                            <li><a href="#">DC</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC Universe</a></li>
                            <li><a href="#">DC Power Visa</a></li>
                        </ul>
                    </div>
                </nav>

                <div class="footer_logo">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>

        <div class="bottom_footer">
            <div class="container"></div>
        </div>
    </footer>
</template>

<script>
export default {
    name : 'Footer'
}
</script>

<style lang="scss" scoped>
@import '../assets/css/variables.scss';

    .top_footer {
        background-color: $primary_color;

        ul {
            padding: 50px 0;
            display: flex;
            justify-content: space-around;
            align-items: center;

            a {
                color: $col_white;
                text-transform: uppercase;
                display: flex;
                align-items: center;

                img {
                    height: 60px;
                    margin-right: 15px;
                }
            }

            li:last-child {
                img {
                    height: 40px;
                }
            }
        }
    }

    .main_footer {
        
        background-image: url('../assets/img/footer-bg.jpg');
        background-size: cover;

        .container {
            height: 400px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            overflow: hidden;

            .footer_nav {
                display: flex;
                .ul_col {
                    margin-right: 30px;

                    #shop {
                        margin-top: 20px;
                    }

                    li {
                        margin: 5px 0;
                    }

                    li:first-child {
                        margin-bottom: 15px;
                    }

                    li:first-child a{
                        font-size: 18px;
                        font-weight: bold;
                        color: $col_white;
                        text-transform: uppercase;
                    }

                    a {
                        color: $text_link_color;
                    }
                }
            }

            img {
                width: 600px;
            }
        }
    }
</style>