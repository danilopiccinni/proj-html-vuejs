<script>
    export default {
        data() {
            return {
                columnAbout: {
                    title: 'about',
                    content : 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Ad dolor et sed ratione, commodi alias, soluta nam natus deleniti maiores perspiciatis dolorum iusto quam fugiat enim excepturi libero aliquam odio!',
                    image : '/img/avada-movers-retinalogo.png'
                },

                columns : [
                    {
                        title : 'avada movers',
                        links : [
                            'home',
                            'Rates',
                            'testimonials',
                            'blog',
                            'free quote'
                        ]

                    },
                    {
                        title : 'recent posts',
                        links : [
                            'heading out to college?',
                            'moving your business?',
                            'outstanding quality',
                            'cost of moving',
                            'best moving tips'
                        ]
                    }
                ]
            }
        }
    }
</script>

<template>
    <footer>
        <div class="container">
            <div class="column-about">
                <strong> {{ columnAbout.title }}</strong>
                <p>{{ columnAbout.content }}</p>
                <img :src="columnAbout.image" alt="">
            </div>

            <div class="cont-columns">
                <div v-for="column in columns" class="column">
                    <strong> {{ column.title }}</strong>
                    <ul>
                        <li v-for="link in column.links">{{ link }}</li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<style scoped lang="scss">

.container {
    display: flex;
    gap: 100px;
    padding: 100px 0;
}

.column-about {
    display: flex;
    flex-direction: column;
    gap: 20px;
    width: 300px;
}

img {
    width: 50%;
}

.cont-columns {
    display: flex;
    gap: 200px;
}

.column {
    display: flex;
    flex-direction: column;
    gap: 20px;

}

ul {
    display: flex;
    flex-direction: column;
    gap: 20px;
    padding-left: 0;
}

li {
    font-size: 15px;
    list-style-type: '> ';
}

strong {
    font-weight: bold;
    text-transform: uppercase;
}



</style>