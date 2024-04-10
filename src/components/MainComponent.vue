<template>
    <main>
        <div class="top-part">
            <div class="container">
                <span> --> Content goes here <-- </span>
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
</style>