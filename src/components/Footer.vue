<template>
    <footer>
        <!-- componente top footer -->
        <TopFooter/>
        <!-- componente footer centrale -->
        <MainFooter/>
        <!-- componente bottom footer con link social -->
        <BottomFooter/>
    </footer>
</template>

<script>
import TopFooter from './footer_components/TopFooter.vue'
import MainFooter from './footer_components/MainFooter.vue'
import BottomFooter from './footer_components/BottomFooter.vue'

export default {
    name : 'Footer',
    components: {
        TopFooter,
        MainFooter,
        BottomFooter
    }
}
</script>

<style>

</style>