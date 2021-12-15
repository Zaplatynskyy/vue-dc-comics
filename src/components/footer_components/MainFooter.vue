<template>
  
    <div class="main_footer">
        <div class="container">
            <!-- link utili footer centrale -->
            <nav class="footer_nav">
                <!-- prima colonna link -->
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

                <!-- seconda colonna link -->
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

                <!-- terza colonna link -->
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

            <!-- logo footer centrale -->
            <div class="footer_logo">
                <img src="../../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </div>

</template>

<script>
export default {
    name : 'MainFooter'
}
</script>

<style lang="scss" scoped>
@import '../../assets/css/variables.scss';

    .main_footer {
        
        background-image: url('../../assets/img/footer-bg.jpg');
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
                    // li:firs-child rappresenta il titolo di ogni colonna dei link utili
                    li:first-child {
                        margin-bottom: 15px;
                    }

                    li:first-child a{
                        font-size: 18px;
                        font-weight: bold;
                        color: $col_white;
                        text-transform: uppercase;

                        &:hover {
                            text-decoration: none;
                            cursor: default;
                        }
                    }

                    a {
                        color: $text_link_color;

                        &:hover {
                            text-decoration: underline;
                        }
                    }
                }
            }

            // dimensioni logo footer
            img {
                width: 600px;
            }
        }
    }

</style>