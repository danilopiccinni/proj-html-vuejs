<script>
    export default {
        data() {
            return {
                persons: [ 
                    {
                        image : '/img/avada-movers-johndoe-final.jpg',
                        name : 'john doe',
                        description : 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Soluta, aliquam ratione aperiam quasi neque nulla tempora ullam, veniam quaerat ex dolor nemo odit sapiente qui quibusdam deleniti obcaecati autem earum!',
                    },
                    {
                        image : '/img/avada-movers-janedoe-final.jpg',
                        name : 'jane doe',
                        description : 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Soluta, aliquam ratione aperiam quasi neque nulla tempora ullam, veniam quaerat ex dolor nemo odit sapiente qui quibusdam deleniti obcaecati autem earum!',
                    },
                    {
                        image : '/img/avada-movers-johnsmith-final.jpg',
                        name : 'john smith',
                        description : 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Soluta, aliquam ratione aperiam quasi neque nulla tempora ullam, veniam quaerat ex dolor nemo odit sapiente qui quibusdam deleniti obcaecati autem earum!',
                    }
                ]
            }
        }
    }
</script>

<template>
    <div class="section4">
        <div class="container padding cont-section4">
            <div>
                <h6>happy customers</h6>
                <h3 class="section-title">testimonials</h3>
            </div>
            <div class="cont-cards flex-column flex-md-row row-cols-sm-1 row-cols-md-4">
                <div v-for="person in persons" class="_card">
                    <img :src="person.image" alt="">
                    <h5> {{ person.name }}</h5>
                    <p> <em>"{{ person.description }}"</em> </p>
                </div>
            </div>
            <div>
                <a class="link" href="">read more testmonials</a>
            </div>
        </div>
    </div>

</template>

<style scoped lang="scss">

.section4 {
    background-image: url(/img/avada-movers-testimonial-background.jpg);
    background-repeat: no-repeat;
    background-position: 50% 25%;
}

img {
    width: 100px;
    border-radius: 50%;
}

.cont-section4 {
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    gap: 50px;
    text-align: center;


}
.cont-cards {
    display: flex;
    justify-content: space-between;
    gap: 50px;
}

._card {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 20px;
    text-align: center;
}

h5 {
    color: #1675bf;
    text-transform: capitalize;
    font-weight: bold;
}

p {
    font-size: 12px;
}

</style>