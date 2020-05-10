<template>
    <div id="app">
        <Home></Home>
    </div>
</template>

<script>
    import Home from './Home.vue'

    export default {
        name: 'App',
        components: {
            Home,
        }
    }


</script>

<style>
    #app {
        justify-content: center;
        align-items: center;
        display: flex;
        position: absolute;
        width: 100%;
        height: 100%;
        /*top:50%;*/
        /*left:50%;*/
        /*transform:translate(-50%,-50%);*/
    }
</style>
