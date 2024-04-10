<template>
    <div>
        bottomfooter
    </div>
</template>

<script>
    export default {
        name: 'bottomFooterComponent'
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

div{
    background-color: $bottomfooterbackground;
    color: white;
}
</style>