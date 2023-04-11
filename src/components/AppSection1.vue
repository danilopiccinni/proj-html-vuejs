<script>
    export default {
        data() {
            return {

            }
        }
    }
</script>

<template>
    <div class="section1">
        <span>headache free</span>
        <h3>award winning</h3>
        <h3>moving company</h3>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Soluta, aliquam ratione aperiam quasi neque nulla tempora ullam, veniam quaerat ex dolor nemo odit sapiente qui quibusdam deleniti obcaecati autem earum!</p>
        <a href="">read our testimonials</a>
    </div>

</template>

<style scoped lang="scss">

    .section1 {
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 10px;

        text-align: center;

        padding: 150px 600px;

        background-color: #F2F5F8;
    }

    h3 {
        color: #6ABF16;
        font-weight: bold;
        text-transform: uppercase;
        
    }

    span{
        color: #333333;
        font-weight: bold;
        text-transform: uppercase;
        margin-bottom: 0;
    }

    a {
        font-size: 12px;
        font-weight: bold;
        text-transform: uppercase;
        text-decoration: none;
        color: white;
        background-color: #1675bf;
        padding: 5px 20px;
        border-radius: 15px;
    }


</style>