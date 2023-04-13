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
                    },
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
                    },
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
                    },
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
                    },
                    
                ]
            }
        },

        methods : {
            avanti() {
                document.querySelector('.scroller').scrollBy({
                    left : 350,
                    behavior : 'smooth'
                })
            },
            indietro() {
                document.querySelector('.scroller').scrollBy({
                    left : -350,
                    behavior : 'smooth'
                })
            },


        },

        mounted() {
            document.querySelector('.scroller').scrollBy({
                        left : 900,
                        behavior : 'smooth'
                    })

            }
        
    }
</script>

<template>

    <div class="section4">
        <div class=" container padding cont-section4">
            <div class="cont-title">
                <h6>happy customers</h6>
                <h3 class="section-title">testimonials</h3>
            </div>
            <div class="scroller">
                <div class="scroller-items">
                    <div v-for="person in persons" class="__card">
                        <div class="cont-img">
                            <img :src="person.image" alt="">
                            <h5> {{ person.name }}</h5>
                            <p> <em>"{{ person.description }}"</em> </p>
                        </div>
                    </div>
                </div>

                <div class="cont-button">
                    <div class="button" @click="indietro()"><i class="fa-solid fa-circle-chevron-left"></i></div>
                    <div class="button" @click="avanti()"><i class="fa-solid fa-circle-chevron-right"></i></div>
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

.cont-section4 {
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    gap: 50px;
    text-align: center;
    position: relative;

}


.scroller {
    padding-top: 25px;

    display: flex;
    justify-content: flex-start;
    align-items: center;
    width: 100%;

    overflow-x: scroll;
    
    -ms-overflow-style: none;  /* IE and Edge */
    scrollbar-width: none; 

}



.button:hover {
    color: #228ddf;
    cursor: pointer;
}

.cont-button{
    color: #1675bf;
    font-size: 35px;
    display: flex;
    gap: 10px;
    position: absolute;
    bottom: 200px;
    left: 50%;

    transform: translateX(-50%);
}

/* Hide scrollbar for Chrome, Safari and Opera */
.scroller::-webkit-scrollbar {
  display: none;
}

/* Hide scrollbar for IE, Edge and Firefox */
.example {
  -ms-overflow-style: none;  /* IE and Edge */
  scrollbar-width: none;  /* Firefox */
}

.scroller-items {
    width: 300px;

    display: flex;
    gap: 50px;
}

.__card {
    width: 300px;
    height: 300px;

    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 20px;
    text-align: center;

    &:hover {
        cursor: pointer;
    }

    &:hover img {
        border: 5px solid #1675bf;
    }
}

.cont-img {
    width: 300px;
    height: 300px;
}

img {
    width: 100px;
    border-radius: 50%;

    transition: 0.1s;
    transition-timing-function: ease-in-out;

     
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
