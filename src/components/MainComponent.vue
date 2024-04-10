<template>
    <main>
        <div class="top-part">
            <div class="container">
                <span> --> Content goes here <-- </span>
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
    export default {
        name: 'MainComponent',
        data() {
            return {
                
            }
        },
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/_variables.scss' as *;
    .top-part{
        background-color: $mainbg;
        color: $white;
        font-weight: 600;
        padding: 40px;
        font-size: 30px;
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