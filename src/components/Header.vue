<template>
    <header>
        <div class="container">
            <!-- img logo header -->
            <a href="#">
                <img src="../assets/img/dc-logo.png" alt="logo dc comics">
            </a>

            <!-- link di collegamento header -->
            <nav class="header_nav">
                <ul>
                    <li><a href="#">Characters</a></li>
                    <li><a href="#" class="selected">Comics</a></li>
                    <li><a href="#">Movies</a></li>
                    <li><a href="#">Tv</a></li>
                    <li><a href="#">Games</a></li>
                    <li><a href="#">Collectibles</a></li>
                    <li><a href="#">Videos</a></li>
                    <li><a href="#">Fans</a></li>
                    <li><a href="#">News</a></li>
                    <li><a href="#">Shop</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name : 'Header'
}
</script>

<style lang="scss" scoped>
@import '../assets/css/variables.scss';

    header {
        height: 120px;
        background-color: $col_white;

        .container {
            height: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            // dimensioni logo
            img {
                    height: 80px;
            }

            // proprietà link di collegamento header
            .header_nav {
                
                ul {

                    li {
                        display: inline-block;

                        a {
                            height: 120px;
                            line-height: 120px;
                            font-weight: bold;
                            color: $text_link_color;
                            text-transform: uppercase;
                            display: inline-block;
                            margin: 0 15px;

                            &:hover {
                                color: $primary_color;
                                border-bottom: 5px solid $primary_color;
                            }

                            &.selected {
                                color: $primary_color;
                                border-bottom: 5px solid $primary_color;
                            }
                        }
                    }
                }
            }
        }
    }
</style>