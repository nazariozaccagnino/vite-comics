<template>
    <div id="middlefooter">
        <div class="container">
            <div class="d-flex justify-content-between ">
                <div>
                    <div class="row p-4">
                        <div class="col-8">
                            <h4>DC COMICS</h4>
                            <ul>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                            </ul>
                            <h4>SHOP</h4>
                            <ul>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                            </ul>
                        </div>
                        <div class="col-2">
                            <h4>DC</h4>
                            <ul>
                                <li>
                                    <a href="#">Terms of Use</a>
                                </li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                            </ul>
                        </div>
                        <div class="col-2">
                            <h4>SITES</h4>
                            <ul>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
                                <li>a</li>
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
        name: 'MiddleFooterComponent'
    }
</script>

<style lang="scss" scoped>
#middlefooter{
    background-image: url(/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    color: white;
    #bigdclogo{
        object-fit: contain;
        width: 50%;
        
    }
    img{
        
    }
}
.container{
    ul{
        list-style: none;
        padding: 0px;
    }
    h4{
        
    }
}
</style>