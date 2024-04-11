<template>
    <div class="card">
        <img :src="image" class="card-img-top thumb" :alt="descr">
        <div class="card-body">
            <p class="card-text">{{descr}}</p>
            <!-- <a href="#" class="btn btn-primary">Go somewhere</a> -->
        </div>
    </div>
</template>

<script>
export default {
    name: 'CardComponent',
    props: ['image', 'price', 'descr', 'type']

}
</script>

<style lang="scss" scoped>
.thumb{
    aspect-ratio: 1 / 1;
}
</style>