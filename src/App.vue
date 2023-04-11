<script>
    import AppSection2 from './components/AppSection2.vue'
    import AppSection1 from './components/AppSection1.vue';
    import AppBannerBlue from './components/AppBannerBlue.vue';
    import AppBannerGreen from './components/AppBannerGreen.vue';
    import AppHeader from './components/AppHeader.vue';
    export default {
        data() {
            return {

            }
        },
        components : {
            AppSection2,
            AppSection1,
            AppBannerBlue,
            AppBannerGreen,
            AppHeader,

        }
    }
</script>

<template>

    <AppBannerGreen></AppBannerGreen>

    <AppHeader></AppHeader>

    <AppBannerBlue></AppBannerBlue>

    <AppSection1></AppSection1>

    <AppSection2></AppSection2>

</template>

<style scoped lang="scss">

</style>
