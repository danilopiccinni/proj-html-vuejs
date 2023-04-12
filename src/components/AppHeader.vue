<script>
import 'animate.css'
import AppNav from './AppNav.vue';
    export default {
        data() {
            return {
                pulseOn : false
            }
        },
        components : {
            AppNav,
        },

        methods : {
            activePulse() {
                this.pulseOn = true
            },

            deactivePulse() {
                this.pulseOn = false
            } 
        }
    }
</script>

<template>
    <header>
        <AppNav></AppNav>

        <div class="titolo" @mouseover="activePulse()" @mouseleave="deactivePulse()" :class="pulseOn == true ? 'animate__animated animate__jello' : ''">
            <h6 class="animate__animated animate__zoomInDown">moving without the hassle</h6>
            <h1 class="animate__animated animate__zoomIn" >we make it simple</h1>
            <h6 class="animate__animated animate__zoomInUp">professional service with quality and customer satisfaction</h6>
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