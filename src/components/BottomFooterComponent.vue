<template>
    <div id="bottomfooter">
        <div class="container">
            bottomfooter
        </div>
    </div>
</template>

<script>
    export default {
        name: 'bottomFooterComponent'
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

#bottomfooter{
    background-color: $bottomfooterbackground;
    color: white;
}
</style>