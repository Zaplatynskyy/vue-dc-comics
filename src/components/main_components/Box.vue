<template>
    <!-- elemento box -->
    <div class="box">
        <!-- img elemento box -->
        <img :src="box.thumb" alt="">
        <!-- titolo elemento box -->
        <div class="title_serie">{{box.series}}</div>
    </div>
</template>

<script>
export default {
    name : 'Box',
    // importo l'oggetto data dall'array 
    props : {
        box : Object
    }
}
</script>

<style lang="scss" scoped>
// import variabili scss
@import '../../assets/css/variables.scss';
    // <!-- elemento box -->
    .box {
        // <!-- img elemento box -->
        img {
            width: 100%;
            height: 230px;
            object-fit: cover;
            object-position: top;
        }
        // <!-- titolo elemento box -->
        .title_serie {
            font-size: 18px;
            text-align: left;
            text-transform: uppercase;
            color: $col_white;
            margin: 10px 0;

        }
    }
</style>