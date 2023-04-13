<script>
    export default {
        data() {
            return {

            }
        }
    }
</script>

<template>
    <div class="cont">
        <div class="container banner">
            <div class="banner-sx">
                <i class="fa-solid fa-phone-flip"></i>
                <span>Call us for a Free Quote: <span class="numero-tel">1.800.555.6789</span> </span>
            </div>
    
            <div class="banner-dx">
                <i class="fa-brands fa-facebook-f"></i>
                <i class="fa-brands fa-twitter"></i>
                <i class="fa-brands fa-instagram"></i>
                <i class="fa-brands fa-youtube"></i>
            </div>
        </div>

    </div>
</template>

<style scoped lang="scss">
.cont{
    padding: 8px 0;
    background-color: #6AAF16;
    color: white;
}
.banner {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.banner-sx {
    display: flex;
    align-items: center;
    gap: 5px;
    font-size: 12px;

}

.banner-dx {
    display: flex;
    gap: 20px;
    font-size: 12px;
}

i:hover{
    cursor: pointer;
}

span:hover {
    cursor: pointer;
}

span:hover .numero-tel {
    text-decoration: underline;
}




</style>