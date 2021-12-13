<template>
    
    <div class="top_footer">
        <div class="container">
            <ul>
                <li>
                    <a href="#">
                        <img src="../../assets/img/buy-comics-digital-comics.png" alt="">
                        <div class="text">digital comics</div>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../../assets/img/buy-comics-merchandise.png" alt="">
                        <div class="text">dc merchandise</div>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../../assets/img/buy-comics-subscriptions.png" alt="">
                        <div class="text">subscription</div>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../../assets/img/buy-comics-shop-locator.png" alt="">
                        <div class="text">comic shop locator</div>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../../assets/img/buy-dc-power-visa.svg" alt="">
                        <div class="text">dc power visa</div>
                    </a>
                </li>
            </ul>
        </div>
    </div>

</template>

<script>
export default {
    name : 'TopFooter'
}
</script>

<style lang="scss" scoped>
@import '../../assets/css/variables.scss';

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
</style>