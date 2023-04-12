<script>
    export default {
        data() {
            return {

                activeIndex : 0,

                navLinks: [
                    'home',
                    'rates',
                    'testimonials',
                    'FAQ',
                    'blog',
                    'contact',
                ]
            }
        },

        methods : {
            giveActive(index) {
                this.activeIndex = index
            }
        }
    }
</script>

<template>
    <nav>
        <div class="container flex-column flex-lg-row cont-nav">
            <div>
                <img src="/img/avada-movers-logo.png" alt="">
            </div>
    
            <div class="nav-dx">
                <ul>
                    <li v-for="link,index in navLinks" @click="giveActive(index)" :class="activeIndex == index ? 'active' : ''"> {{ link }}</li>
                    <a class="link d-none d-lg-block" href="">free quote</a>
                </ul>

            </div>
        </div>
    </nav>
</template>

<style scoped lang="scss">

.cont-nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    
    ul {
        display: flex;
        align-items: center;
        gap: 50px;
        list-style-type: none;
    }

    li {
        font-size: 12px;
        font-weight: bold;
        text-transform: capitalize;

        transition: 0.5s;

        &:hover {
            scale: 115%;
            cursor: pointer;
        }

    }

    .active{
        color: #6abf16;
    }

}
</style>