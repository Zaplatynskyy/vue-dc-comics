<template>
    <div class="box">
        <img :src="box.thumb" alt="">
        <div class="title_serie">{{box.series}}</div>
    </div>
</template>

<script>
export default {
    name : 'Box',
    props : {
        box : Object
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/css/variables.scss';

    .box {
        img {
            width: 100%;
            height: 230px;
            object-fit: cover;
            object-position: top;
        }

        .title_serie {
            font-size: 18px;
            text-align: left;
            text-transform: uppercase;
            color: $col_white;
            margin: 10px 0;

        }
    }
</style>