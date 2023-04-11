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
                    'FREE QOUTE',

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
    
            <div>
                <ul>
                    <li v-for="link in navLinks"> {{ link }}</li>
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

    li:last-child {
        color: white;
        background-color: #1675BF;
        border-radius: 15px;
        padding: 5px 15px ;
    }
}
</style>