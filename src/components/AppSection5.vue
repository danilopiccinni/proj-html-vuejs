<script>
    export default {
        data() {
            return {

            }
        }
    }
</script>

<template>
    <div class="section5">
        <div class="container">
            <h3>request a free quote</h3>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ullam omnis ipsam perspiciatis dolore quisquam illum nulla pariatur dolorem qui quos similique doloremque voluptas adipisci, delectus eveniet incidunt, voluptatibus minima earum.</p>
            <a href="">click here</a>
        </div>
    </div>

</template>

<style scoped lang="scss">
    .section5 {
        height: 500px;
        background-image: url(/img/avada-movers-request-quote-background.jpg);
        background-repeat: no-repeat;
        background-size: cover;

        border-bottom: 10px solid #6abf16;
    }

    .container {
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 20px;
        text-align: center;

    }

    h3 {
        font-size: 40px;
        font-weight: bold;
        text-transform: capitalize;
        color: #6abf16;
    }
    a {
    color: white;
    text-decoration: none;

    font-size: 12px;
    text-transform: uppercase;
    font-weight: bold;

    background-color: #1675bf;
    padding: 8px 20px;
    border-radius: 15px;
}

</style>