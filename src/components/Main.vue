<template>
    <main class="debug">
        <div id="jumbotron">

        </div>

        <div id="main_content">
            <div class="container">

            </div>
        </div>
    </main>
</template>

<script>
export default {
    name : 'Main'
}
</script>

<style lang="scss" scoped>
@import '../assets/css/variables.scss';

    #jumbotron {
        height: 400px;
        background-image: url('../assets/img/jumbotron.jpg');
        background-size: cover;
    }

    #main_content {
        background-color: $bg_main;
    }
</style>