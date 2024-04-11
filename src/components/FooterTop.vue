<template>
    <div class="footer-top">
        <div class="container d-flex justify-content-between ">
            <div class="d-flex">
                <div class="menu">
                    <ul>
                        <span>DC Comics</span>
                        <li v-for="(item, index) in dcComics">
                            <a :href="item.url">{{ item.name }}</a>
                        </li>
                    </ul>
                    <ul>
                        <span>Shop</span>
                        <li v-for="(item, index) in shop">
                            <a :href="item.url">{{ item.name }}</a>
                        </li>
                    </ul>
                </div>
                <div class="menu">
                    <ul>
                        <span>DC</span>
                        <li v-for="(item, index) in dc">
                            <a :href="item.url">{{ item.name }}</a>
                        </li>
                    </ul>
                </div>
                <div class="menu">
                    <ul>
                        <span>Sites</span>
                        <li v-for="(item, index) in sites">
                            <a :href="item.url">{{ item.name }}</a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="logo">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name:'FooterTop',
        data() {
            return {
                dcComics: [
                    {
                        name: 'Characters',
                        url: '#'
                    },
                    {
                        name: 'Comics',
                        url: '#'
                    },
                    {
                        name: 'Movies',
                        url: '#'
                    },
                    {
                        name: 'TV',
                        url: '#'
                    },
                    {
                        name: 'Games',
                        url: '#'
                    },
                    {
                        name: 'Videos',
                        url: '#'
                    },
                    {
                        name: 'News',
                        url: '#'
                    }
                ],
                shop: [
                    {
                        name: 'Shop DC',
                        url: '#'
                    },
                    {
                        name: 'Shop DC Collectibles',
                        url: '#'
                    }
                ],
                dc: [
                    {
                        name: 'Terms Of Use',
                        url: '#'
                    },
                    {
                        name: 'Privacy policy (New)',
                        url: '#'
                    },
                    {
                        name: 'Ad Choices',
                        url: '#'
                    },
                    {
                        name: 'Advertising',
                        url: '#'
                    },
                    {
                        name: 'Jobs',
                        url: '#'
                    },
                    {
                        name: 'Subscriptions',
                        url: '#'
                    },
                    {
                        name: 'Talent Workshop',
                        url: '#'
                    },
                    {
                        name: 'CPSC Certificates',
                        url: '#'
                    },
                    {
                        name: 'Ratings',
                        url: '#'
                    },
                    {
                        name: 'Shop Help',
                        url: '#'
                    },
                    {
                        name: 'Contact Us',
                        url: '#'
                    }
                ],
                sites: [
                    {
                        name: 'DC',
                        url: '#'
                    },
                    {
                        name: 'MAD Magazine',
                        url: '#'
                    },
                    {
                        name: 'DC Kids',
                        url: '#'
                    },
                    {
                        name: 'DC Universe',
                        url: '#'
                    },
                    {
                        name: 'DC Power Visa',
                        url: '#'
                    }
                ],
            }
        },
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/_variables.scss' as *;
    .footer-top{
        background-image: url('../assets/img/footer-bg.jpg');
        background-repeat: no-repeat;
        background-size: cover;
    }

    ul{
        padding-top: 20px;

        span{
            color: $white;
            text-transform: uppercase;
            font-weight: 600;
            font-size: 17px;
        }

        li{
            padding-top: 3px;
            font-size: 14px;
            a{
                text-decoration: none;
                color: $grayfootertext;
            }
        }
    }

    .logo{
        margin-top: -95px;

        img{
            width: 105%;
        }
    }

    // .logo {
    //     width: 500px;
    // }

    // .logo img {
    //     position: absolute;
    //     right: 100px;
    //     top: 300px;
    // }

</style>