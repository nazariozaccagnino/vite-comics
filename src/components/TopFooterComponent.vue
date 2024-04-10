<template>
    <div id="topfooter">
        <div class="container">
            <ul>
                <li v-for="(item, index) in buylist">
                    <div class="d-flex">
                        <img :src="'/img/'+item.img" alt="">
                        <div class="description">{{ item.name }}</div>
                    </div>                    
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'TopFooterComponent',
    
    data(){
        return{
            buylist:[
                {
                    name: 'digital comics',
                    img: 'buy-comics-digital-comics.png'
                },
                {
                    name: 'dc merchandise',
                    img: 'buy-comics-merchandise.png'
                },
                {
                    name: 'subscription',
                    img: 'buy-comics-subscriptions.png'
                },
                {
                    name: 'comic shop locator',
                    img: 'buy-comics-shop-locator.png'
                },
                {
                    name: 'dc power visa',
                    img: 'buy-dc-power-visa.svg'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

#topfooter{
    background-color: $topfooterbackground;
    padding: 20px;
    ul{
        list-style: none;
        display: flex;
        justify-content: center;
        li{
            padding: 10px;
        }
        li img{
            width: 50px;
            height: 50px;
            object-fit: contain;
        }
        .description{
            align-self: center;
            text-transform: uppercase;
            font-weight: 300;
            color: white;
            padding: 5px;
        }
    }
}
</style>