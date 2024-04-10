<template>
   <div class="container d-flex justify-content-between">
        <div>
            <img src="/img/dc-logo.png" alt="logo">
        </div>
        <div class="d-flex">
            <ul>
                <li class="d-flex align-items-center" v-for="(item, index) in menulist" :key="menu">
                    <a :href="item.link">{{ item.name }}</a>
                </li>
            </ul>
        </div>
   </div>
</template>

<script>
    export default {
        name: 'HeaderComponent',
    
    data(){
        return{
            menulist:[
                {
                    name: 'characters',
                    link: '#'
                },
                {
                    name: 'comics',
                    link: '#'
                },
                {
                    name: 'movies',
                    link: '#'
                },
                {
                    name: 'tv',
                    link: '#'
                },
                {
                    name: 'games',
                    link: '#'
                },
                {
                    name: 'collectibles',
                    link: '#'
                },
                {
                    name: 'videos',
                    link: '#'
                },
                {
                    name: 'fans',
                    link: '#'
                },
                {
                    name: 'news',
                    link: '#'
                },
                {
                    name: 'shop',
                    link: '#'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.container img{
    padding: 10px 0;
}
ul{
    list-style: none;
    display: flex;
    height: 100%;
    li{
        padding: 0px 5px,
        
    }
    a{
        text-decoration: none;
        color: black;
        text-transform: uppercase;
        font-weight: 500;
    }
    li:hover{
        border-bottom: 5px solid blue;
    }
    a:hover{
        color: blue;
    }
}
</style>