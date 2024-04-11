<template>
    <div>
        <div class="square">
            <img :src="thumb" :alt="type">
        </div>
        <p>{{ series }}</p>
        <p>Costo: {{ price }}</p>
    </div>
</template>

<script>
    export default {
        name: 'CardComponent',
        props: ['thumb', 'price', 'series','type']
    }
</script>

<style lang="scss" scoped>
    .square{
        height: 200px;
        width: 200px;
        overflow: hidden;

        img{
            width: 100%;
        }
    }

    p{
        font-size: 17px;
        text-transform: uppercase;
    }
</style>