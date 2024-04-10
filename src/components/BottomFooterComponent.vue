<template>
    <div id="bottomfooter">
        <div class="container d-flex justify-content-between">
            <div id="signup">
                <p>sign-up now!</p>
            </div>
            <div class="d-flex align-items-center">
                <div id="followus">
                    follow us
                </div>
                <div id="socials">
                    <img src="/img/footer-facebook.png" alt="facebook">
                    <img src="/img/footer-twitter.png" alt="twitter">
                    <img src="/img/footer-youtube.png" alt="youtube">
                    <img src="/img/footer-periscope.png" alt="periscope">
                    <img src="/img/footer-pinterest.png" alt="pinterest">

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
#followus{
    padding: 0px 20px;
    text-transform: uppercase;
    font-weight: 600;
    font-size: 1.3rem;
    color: $topfooterbackground;
}
#socials{
    img{
        padding: 0px 10px;
    }
}
</style>