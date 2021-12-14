<template>
  
    <div class="bottom_footer">
        <div class="container">

            <button class="btn">Sign-up now!</button>

            <ul class="social_nav">
                <li><a href="#">Follow us</a></li>
                <li><a href="#"><img src="../../assets/img/footer-facebook.png" alt=""></a></li>
                <li><a href="#"><img src="../../assets/img/footer-twitter.png" alt=""></a></li>
                <li><a href="#"><img src="../../assets/img/footer-youtube.png" alt=""></a></li>
                <li><a href="#"><img src="../../assets/img/footer-periscope.png" alt=""></a></li>
                <li><a href="#"><img src="../../assets/img/footer-pinterest.png" alt=""></a></li>
            </ul>

        </div>
    </div>

</template>

<script>
export default {
    name : 'BottomFooter'
}
</script>

<style lang="scss" scoped>
@import '../../assets/css/variables.scss';

    .bottom_footer {
        background-color: $secondary_color;

        .container {    
            padding: 30px 0;
            display: flex;
            justify-content: space-between;

            .btn {
                color: white;
                font-weight: bold;
                text-transform: uppercase;
                background-color: $secondary_color;
                border: 1px solid $primary_color;
                padding: 10px;
                cursor: pointer;

                &:hover {
                    background-color: black;
                }
            }

            .social_nav {
                li {
                    vertical-align: middle;
                    display: inline-block;
                    margin: 0 10px;
                }

                li:first-child a {
                    color: $primary_color;
                    font-weight: bold;
                    text-transform: uppercase;
                }
            }
        }
    }
</style>