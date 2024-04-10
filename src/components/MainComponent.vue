<template>
    <main>
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
</style>