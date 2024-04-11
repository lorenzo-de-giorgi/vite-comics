<template>
    <main>
        <div class="jumbo"></div>
        <div class="top-part">
            <div class="container">
                <div class="t-y">
                    <span class="current-series">Current Series</span>
                </div>
                <div class="row">
                    <div class="col-12 col-md-6 col-lg-3 col-xl-2 mb-4" v-for="(item, index) in comics" :key="index">
                        <CardComponent :thumb="item.thumb" :series="item.series" :price="item.price" :type="item.type" />
                    </div>
                </div>
                <div class="text-center">
                    <button class="more">load more</button>
                </div>
            </div>
        </div>
        <div class="bottom-part">
            <div class="container d-flex justify-content-center align-items-center">
                <div>
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                    <span>Digital Comics</span>
                </div>
                <div>
                    <img src="../assets/img/buy-comics-merchandise.png" alt="">
                    <span>DC Merchandise</span>
                </div>
                <div>
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                    <span>Subscription</span>
                </div>
                <div class="img-locator">
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                    <span>Comic Shop Locator</span>
                </div>
                <div>
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                    <span>DC Power Visa</span>
                </div>
            </div>
        </div>
    </main>
</template>

<script>
    import { comics } from '../data/store.js';
    import CardComponent from './CardComponent.vue';
    export default {
        name: 'MainComponent',
        components: {
            CardComponent
        },
        data() {
            return {
                comics: comics
            }
        },
        mounted() {
            console.log(this.comics)
        },
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/_variables.scss' as *;

    .jumbo{
            background-image: url('../assets/img/jumbotron.jpg');
            background-size: cover;
            background-repeat: no-repeat;
            height: 400px;
            width: 100%;
    }

    .top-part{
        background-color: $mainbg;
        color: $white;
        font-weight: 600;
        padding: 40px;
        font-size: 30px;
    }

    .t-y{
        transform: translateY(-140%);
    }

    .current-series{
        background-color: $bluetext;
        padding: 10px 30px;
        text-transform: uppercase;
        font-size: 20px;
        font-weight: 700;
    }

    .more{
        text-transform: uppercase;
        font-size: 16px;
        padding: 8px 45px;
        background-color: $bluetext;
        color: $white;
        border: none;
        font-weight: 600;
    }

    main{
        position: relative;
    }

    .bottom-part{
        background-color: $bluetext;
        color: $white;

        .container{
            div{
                margin-right: 50px;
            }
        }

        img{
            width: 50px;
            padding-top: 30px;
            padding-bottom: 30px;
        }

        span{
            text-transform: uppercase;
            font-size: 14px;
            margin-left: 15px;
        }

        .img-locator{
            img{
                width: 40px;
            }
        }
    }
</style>