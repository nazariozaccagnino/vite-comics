<template>
    <div id="middlefooter">
        <div class="container">
            <img src="/img/dc-logo-bg.png" alt="">
        </div>
    </div>
</template>

<script>
    export default {
        name: 'MiddleFooterComponent'
    }
</script>

<style lang="scss" scoped>
#middlefooter{
    background-image: url(/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    color: white;
    height: 500px;
    img{
        object-fit: contain;

    }
}
</style>