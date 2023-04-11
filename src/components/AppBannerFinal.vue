<script>
    export default {
        data() {
            return {
                links : [
                    '&copy Copiright 2012 - 2020',
                    'Avada Theme by Theme',
                    'All Rights Reserved',
                    'Powered by WordPress'
                ],

                socials : [
                    '<i class="fa-brands fa-facebook-f"></i>',
                    '<i class="fa-brands fa-twitter"></i>',
                    '<i class="fa-brands fa-instagram"></i>',
                    '<i class="fa-brands fa-youtube"></i>',
                ]
            }
        }
    }
</script>

<template>
    <div class="cont">
        <div class="top">
            <span v-for="link in links" v-html="link"></span>
        </div>
    
        <div class="bottom">
            <span v-for="social in socials" v-html="social"></span>
        </div>
    </div>

</template>

<style scoped lang="scss">

    .cont {
        display: flex;
        flex-direction: column;
        align-items: center;

        gap: 20px;
        background-color: #6abf16;

        padding: 20px 0;
    }

    .top {
        color: white;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 25px;
    }

    .bottom {
        color: white;
        display: flex;
        gap: 25px;
    }

</style>