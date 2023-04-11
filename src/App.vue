<script>
    import AppSection4 from './components/AppSection4.vue';
    import AppSection3 from './components/AppSection3.vue';
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
            AppSection4,
            AppSection3,
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

    <AppSection3></AppSection3>

    <AppSection4></AppSection4>

</template>

<style scoped lang="scss">

</style>
