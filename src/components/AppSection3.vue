<script>
    export default {
        data() {
            return {
                card: 
                    {
                        smallTitle : 'we remove the headache from moving',
                        title : 'move whit ease',
                        description : 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Soluta, veniam quaerat ex dolor nemo odit sapiente qui quibusdam deleniti obcaecati autem earum!',
                    },
            }
        }
    }
</script>

<template>
    <div class="section3">
        <div class="container padding cont-section3">
            <div class="_card">
                <h6> {{ card.smallTitle }}</h6>
                <h3> {{ card.title }}</h3>
                <hr>
                <p> {{ card.description }}</p>
                <a class="link" href="">get a free quote now</a>
            </div>
        </div>
    </div>

</template>

<style scoped lang="scss">

.section3 {
    height: 750px;
    background-image: url(/img/avada-movers-movewithease-background-new.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: top;
}

.cont-section3 {
    height: 100%;
    display: flex;
    justify-content: end;
    align-items: center;
}

._card {
    display: flex;
    flex-direction: column;
    justify-content: center;
    text-align: center;
    width: 450px;
    background-color: #6abf16;

    border: 10px solid #539511;

    padding: 25px;

    color: white;
}

h3 {
    font-size: 35px;
    text-transform: capitalize;
    font-weight: bold;
}

h6 {
    text-transform: uppercase;
    font-size: 10px;
}



</style>