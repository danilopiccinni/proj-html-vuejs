<script>
    export default {
        data() {
            return {

                active : null,

                cards: [ 
                    {
                        image : '/img/avada-movers-serviceonephoto-final.jpg',
                        title : 'two man teams',
                        description : 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Soluta, aliquam ratione aperiam quasi neque nulla tempora ullam, veniam quaerat ex dolor nemo odit sapiente qui quibusdam deleniti obcaecati autem earum!',
                    },
                    {
                        image : '/img/avada-movers-servicetwophoto-final.jpg',
                        title : 'we do all the lifting',
                        description : 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Soluta, aliquam ratione aperiam quasi neque nulla tempora ullam, veniam quaerat ex dolor nemo odit sapiente qui quibusdam deleniti obcaecati autem earum!',
                    },
                    {
                        image : '/img/avada-movers-servicethreephoto-final.jpg',
                        title : 'coast to coast',
                        description : 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Soluta, aliquam ratione aperiam quasi neque nulla tempora ullam, veniam quaerat ex dolor nemo odit sapiente qui quibusdam deleniti obcaecati autem earum!',
                    }
                ]
            }
        }
    }
</script>

<template>
    <div class="section2">
        <div class="container padding cont-section2">
            <div>
                <h6>happy customers</h6>
                <h3 class="section-title">full-service solution</h3>
            </div>
            <div class="cont-cards">
                <div v-for="card,index in cards" class="_card" @mouseover="active=index" @mouseleave="active=null" :style="index == active || active==null ? { opacity: 1}: {opacity : 0.5} ">
                    <img :src="card.image" alt="">
                    <h5>{{ card.title }}</h5>
                    <p>{{ card.description }}</p>
                    <a class="link" href="">read more</a>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">

.cont-section2 {
    display: flex;
    flex-direction: column;
    gap: 50px;
    text-align: center;


}


    .cont-cards {
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
        gap: 15px;

        
    }

    ._card {
        display: flex;
        flex-direction: column;
 
        width: calc(100% / 3 - 15px / 3 * 2);
        min-width: 300px;

        text-align: center;

        padding-bottom: 15px;

        border: 10px solid #f2f5f8;
        transition: 1s;
        transition-timing-function: ease;
        overflow: hidden;

        &:hover {
            border: 10px solid #6abf16;
            transform: scale(105%);
 
        }

        &:hover img {
            scale: 110%;
        }
    }

    img {
        border-bottom: 10px solid #f2f5f8;
        transition: 1s;
    }

    h5 {
        font-size: 20px;
        font-weight: bold;
        color: #1675bf;
        padding-top: 30px;
        text-transform: uppercase;
    }

</style>