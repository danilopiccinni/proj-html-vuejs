<script>
import AppNav from './AppNav.vue';
    export default {
        data() {
            return {

            }
        },
        components : {
            AppNav,
        }
    }
</script>

<template>
    <header>
        <AppNav></AppNav>

        <div class="titolo">
            <h6>moving without the hassle</h6>
            <h1>we make it simple</h1>
            <h6>professional service with quality and customer satisfaction</h6>
        </div>
    </header>

</template>

<style scoped lang="scss">
header {
    height: 600px;
    padding-top: 15px;

    background-image: url(/img/avada-movers-homeherobackground-final.jpg);
    background-position: top;
    background-repeat: no-repeat;
    background-size: cover;
}
.titolo {
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    text-transform: uppercase;

}

h1 {
    font-size: 45px;
    font-weight: bold;
}

h6 {
    color: #333333;
    font-size: 10px;
    font-weight: bold;
}
</style>