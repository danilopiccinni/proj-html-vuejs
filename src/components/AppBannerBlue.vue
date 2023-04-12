<script>
import 'animate.css'
    export default {
        data() {
            return {
                animationOn : false
            }
        },

        methods : {
            activeAnimation() {
                this.animationOn = true
            },

            deactiveAnimation() {
                this.animationOn = false
            }
        }
    }
</script>

<template>
    <div class="banner-blue" @mouseover="activeAnimation()" @mouseleave="deactiveAnimation()">
        
        <span :class="animationOn == true ? 'animate__animated animate__pulse animate__infinite' : ''"><i class="fa-regular fa-paper-plane" ></i> get a free quote online now!</span>
    </div>
</template>

<style scoped lang="scss">

.banner-blue {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 15px;

    height: 100px;
    color: white;
    background-color: #1675BF;

    &:hover {
        cursor: pointer;
        background-color: #2e9cf0;
    }

    span {
        text-transform: uppercase;
    }
}

</style>