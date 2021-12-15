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
                    <li v-for="(link,i) in headerLinks" :key="i"><a :href="link.url" :class="{selected: link.selected}">{{link.title}}</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name : 'Header',
    data() {
        return {
            // array di link di collegamento header
            headerLinks : [
                {
                    url: '#',
                    title : 'Characters',
                    selected : false
                },
                {
                    url: '#',
                    title : 'Comics',
                    selected : true
                },
                {
                    url: '#',
                    title : 'Movies',
                    selected : false
                },
                {
                    url: '#',
                    title : 'Tv',
                    selected : false
                },
                {
                    url: '#',
                    title : 'Games',
                    selected : false
                },
                {
                    url: '#',
                    title : 'Collectibles',
                    selected : false
                },
                {
                    url: '#',
                    title : 'Videos',
                    selected : false
                },
                {
                    url: '#',
                    title : 'Fans',
                    selected : false
                },
                {
                    url: '#',
                    title : 'News',
                    selected : false
                },
                {
                    url: '#',
                    title : 'Shop',
                    selected : false
                }
            ]
        }
    }
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