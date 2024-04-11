<template>
    <div id="middlefooter">
        <div class="container">
            <div class="d-flex justify-content-between">
                <div v-for="(item, index) in actions" :key="index" class="prova">
                    <div>
                        <h5>{{ item.title }}</h5>
                        <ul>
                            <li v-for="(link, index) in item.links" :key="index"><a href="#">{{ link }}</a></li>
                        </ul>
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
    max-height: 450px;
    color: white;

    #bigdclogo {
        object-fit: contain;
        border: 1px solid red;
        height: 400px;
        object-fit: fill;

    }

    #bigdclogo img {
        transform: translate(0%, -5%);
        width: 100%;
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