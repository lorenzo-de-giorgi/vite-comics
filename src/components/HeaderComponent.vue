<template>
    <header class="container">
        <div id="dc-logo">
            <img src="../assets/img/dc-logo.png" alt="logo DC">
        </div>
        <nav>
            <ul>
                <li v-for="(item, index) in nav" :key="index">
                    <a :href="item.url">{{ item.name }}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
    export default {
        data() {
            return {
                nav:[
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
                        name: 'Tv',
                        url: '#'
                    },
                    {
                        name: 'Games',
                        url: '#'
                    },
                    {
                        name: 'Collectibles',
                        url: '#'
                    },
                    {
                        name: 'Videos',
                        url: '#'
                    },
                    {
                        name: 'Fans',
                        url: '#'
                    },
                    {
                        name: 'News',
                        url: '#'
                    },
                    {
                        name: 'Shop',
                        url: '#'
                    },
                ]
            }
        },
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/_variables.scss' as *;
    header{
        display: flex;
        justify-content: space-between;
    }

    img{
        padding: 20px;
        width: 120px;
    }

    nav{
        align-content: center;

        ul{
            list-style: none;
            display: flex;

            li{
                margin: 0 13px;
                a{
                    text-decoration: none;
                    text-transform: uppercase;
                    font-weight: 500;
                    color: $headertext;
                    padding-bottom: 53px;
                    
                    &:hover{
                        transition: 0.1s;
                        border-bottom: 5px solid $bluetext;
                        color: $bluetext;
                    }
                }
            }
        }
    }
</style>