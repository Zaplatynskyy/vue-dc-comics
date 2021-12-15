<template>
    <main>
        <!-- sezione jumbotron -->
        <div id="jumbotron">

        </div>

        <!-- sezione corpo main della pagina -->
        <div id="main_content">
            <div class="container">
                <!-- bottone fissato in alto a sinistra 'current series' -->
                <button class="btn current">Current Series</button>

                <div class="row">
                    <!-- componente Box del singolo elemento -->
                    <Box  v-for="(box,i) in boxs" :key="i" :box="box"/>
                </div>

                <!-- bottone fissato in basso 'load more' -->
                <button class="btn load">Load More</button>
            </div>
        </div>
    </main>
</template>

<script>
import Box from './main_components/Box.vue'
// import array degli elementi comic book dal file json fornito
import array from '../../dc-comics.json'

export default {
    name : 'Main',
    components : {
        Box,
    },
    data() {
        return {
            // array data degli elementi comic book
            boxs : array
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/css/variables.scss';

    // sezione jumbotron
    #jumbotron {
        height: 400px;
        background-image: url('../assets/img/jumbotron.jpg');
        background-size: cover;
    }

    // <!-- sezione corpo main della pagina -->
    #main_content {
        background-color: $bg_main;

        .container {
            text-align: center;
            position: relative;
            padding: 20px 0;

            .btn {
                background-color: $primary_color;
            }

            // bottone fissato in alto a sinistra 'current series'
            .btn.current {
                font-size: 18px;
                padding: 10px 20px;
                position: absolute;
                top: -20px;
                left: 0;
            }

            .row {
                display: flex;
                flex-wrap: wrap;
                justify-content: space-around;

                // dimensioni elemento box
                .box {
                    width: calc(100% / 6 - 20px);
                    margin: 20px 0;
                }
            }

            // bottone fissato in basso 'load more'
            .btn.load {
                padding: 10px 40px;
            }
        }
    }
</style>