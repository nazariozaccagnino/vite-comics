<template>
    <div id="bottomfooter">
        <div class="container d-flex justify-content-between">
            <div id="signup">
                <p>sign-up now!</p>
            </div>
            <div>
                <div id="follow">
                    follow us
                </div>
            </div>
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
#signup{
    border: 2px solid $topfooterbackground;
    padding: 5px;
    margin: 20px;
    p{
        padding: 10px;
        margin: 0;
        text-transform: uppercase;
        font-weight: 600;

    }
}
</style>