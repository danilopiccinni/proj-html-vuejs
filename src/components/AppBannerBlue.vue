<script>
    export default {
        data() {
            return {

            }
        }
    }
</script>

<template>
    <div class="banner-blue">
        <i class="fa-regular fa-paper-plane"></i>
        <span>get a free quote online now!</span>
    </div>
</template>

<style scoped lang="scss">

.banner-blue {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 15px;

    height: 100px;
    color: white;
    background-color: #1675BF;

    &:hover {
        cursor: pointer;
        background-color: #2e9cf0;
    }

    span {
        text-transform: uppercase;
    }
}

</style>