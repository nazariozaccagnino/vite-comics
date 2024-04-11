<template>
    <main>
        <div id="jumbotron">
            <img src="/img/jumbotron.jpg" alt="">
        </div>
        <div id="currentseries">
            current series
        </div>
        <div class="container">
            <div class="row">
                <div class="col-2 d-flex align-items-stretch p-2" v-for="(item, index) in comics">
                    <div class="card">
                        <img :src="item.thumb" class="card-img-top thumb" :alt="item.series">
                        <div class="card-body">
                            <p class="card-text">{{ item.series }}</p>
                            <!-- <a href="#" class="btn btn-primary">Go somewhere</a> -->
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>

<script>
import { comics } from '../data/store.js'
export default {
    name: 'MainComponent',
    data() {
        return {
            comics: comics,
        }
    },
    mounted() {
        console.log(comics);
    }
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

main {
    background-color: $mainbackground;
}

#jumbotron img {
    height: 400px;
    width: 100%;
    object-fit: cover;
    object-position: top 0px left 0px;
}

#currentseries {
    background-color: $topfooterbackground;
    display: inline-block;
    padding: 10px;
    text-transform: uppercase;
    transform: translate(250%, -50%);
    font-weight: 700;
    color: white;
}
.thumb{
    aspect-ratio: 1 / 1;
}
</style>