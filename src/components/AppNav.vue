<script>
    export default {
        data() {
            return {
                navLinks: [
                    'home',
                    'rates',
                    'testimonials',
                    'FAQ',
                    'blog',
                    'contact',
                ]
            }
        }
    }
</script>

<template>
    <nav>
        <div class="container cont-nav">
            <div>
                <img src="/img/avada-movers-logo.png" alt="">
            </div>
    
            <div class="nav-dx">
                <ul>
                    <li v-for="link in navLinks"> {{ link }}</li>
                    <a class="link" href="">free quote</a>
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
    }

    

}
</style>