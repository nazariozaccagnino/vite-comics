<template>
    <div id="middlefooter">
        <div class="container">
            <div class="d-flex justify-content-between">
                <div class="my-4">
                    <div class="row">
                        <div class="col" v-for="(item, index) in actions" :key="index">
                            <h5>{{ item.title }}</h5>
                            <ul>
                                <li v-for="(link, index) in item.links" :key="index"><a href="#">{{ link}}</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div id="bigdclogo">
                    <img src="/img/dc-logo-bg.png" alt="">
                </div>

            </div>

        </div>
    </div>
</template>

<script>
export default {
    name: 'MiddleFooterComponent',
    data() {
        return {
            actions: [
                {
                    title: 'dc comics',
                    links: [
                        'Characters',
                        'Comics',
                        'Movies',
                        'TV',
                        'Games',
                        'Videos',
                        'News'
                    ]
                },
                {
                    title: 'shop',
                    links: [
                        'Shop DC',
                        'Shop DC Collectibles'
                    ]
                },
                {
                    title: 'dc',
                    links: [
                        'Terms Of Use',
                        'Privacy policy (New)',
                        'Ad Choices',
                        'Advertising',
                        'Jobs',
                        'Subscriptions',
                        'Talent Workshops',
                        'CPSC Certificates',
                        'Ratings',
                        'Shop Help',
                        'Contact Us'
                    ]
                },
                {
                    title: 'sites',
                    links: [
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        'DC Power Visa'
                    ]
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

#middlefooter {
    background-image: url(/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    color: white;

    #bigdclogo {
        overflow: hidden;

    }

    #bigdclogo img {
        width: 70%;
        transform: scale(1.3) translate(50px,0px);
    }

}

.container {
    ul {
        list-style: none;
        padding: 0px;
    }

    li {
        color: white;

        a {
            text-decoration: none;
            color: grey
        }
    }

    h5 {
        text-transform: uppercase;
    }
}
.prova{
    display: flex;
    justify-content: space-between;
}
</style>