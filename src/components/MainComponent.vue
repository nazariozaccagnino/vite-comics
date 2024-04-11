<template>
    <main>
        <div id="jumbotron">
            <img src="/img/jumbotron.jpg" alt="">
        </div>
        <div id="currentseries">
            current series
        </div>
        <div class="container">
            >>>Content goes here<<<
        </div>
    </main>
</template>

<script>
    export default {
        name: 'MainComponent'
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

main{
    background-color: $mainbackground;
     div{
        color: white;
     }
}
#jumbotron img{
    height: 400px;
    width: 100%;
    object-fit: cover;
    object-position: top 0px left 0px;
}
#currentseries{
    background-color: $topfooterbackground;
    display: inline-block;
    padding: 10px;
    text-transform: uppercase;
    transform: translate(250%, -50%);
    font-weight: 700;
}
</style>