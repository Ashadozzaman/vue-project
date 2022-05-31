<template>
<img alt="Vue logo" src="./assets/logo.png">
<HelloWorld msg="Welcome to My first Vue.js App" />
<!-- <HomeVue /> -->
<Ashadozzaman />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
// import HomeVue from './components/Home.vue'
import Ashadozzaman from './components/Ashadozzaman.vue'

export default {
    name: 'App',
    components: {
        HelloWorld,
        // HomeVue,
        Ashadozzaman
    }
}
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
