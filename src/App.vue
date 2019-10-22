<template>
    <div id="app">
<!--        <DatePicker/>-->
        <img alt="Vue logo" src="./assets/logo.png">
        <TestBinding msg="I am a test binding"/>
        <Tree />
    </div>
</template>

<script>
    import Vue from 'vue';
    import TestBinding from "@/components/TestBinding";
    import Tree from "@/components/Tree"

    Vue.config.productionTip = false;
    export default {
        name: 'app',
        components: {
          TestBinding, Tree
        }

    }
</script>

<style>
    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }
</style>
