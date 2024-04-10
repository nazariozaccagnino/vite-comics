<template>
    <div id="topfooter">
        <div class="container">
            topfooter
        </div>
    </div>
</template>

<script>
    export default {
        name: 'TopFooterComponent'
    }
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

#topfooter{
    background-color: $topfooterbackground;
}
</style>