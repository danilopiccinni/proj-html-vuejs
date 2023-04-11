<script>
    export default {
        data() {
            return {
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
            <div v-for="card in cards" class="_card">
                <img :src="card.image" alt="">
                <h5>{{ card.title }}</h5>
                <p>{{ card.description }}</p>
                <a class="link" href="">read more</a>
            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">

    .cont-section2 {
        height: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        flex-wrap: wrap;

        
    }

    ._card {
        display: flex;
        flex-direction: column;

        width: 300px;
        height: 500px;

        text-align: center;

        border: 10px solid #f2f5f8;
    }

    img {
        border-bottom: 10px solid #f2f5f8;
    }

    h5 {
        font-size: 20px;
        font-weight: bold;
        color: #1675bf;
        padding-top: 30px;
        text-transform: uppercase;
    }

</style>