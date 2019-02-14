<template>
   <div>
        <NavBar/>
       <div class="w-50 mx-auto border">
           <Caroussel/>
       </div>
       <div class="text-center">
           Passione par le dessin nous nous sommes lance dans la confeciton de teshirt et de badges
           nous proposons une gamme unique et personalisable
       </div>
       <div class="d-flex flex-wrap w-100 justify-content-center bg-light">
          <TeeShirtCard v-for="n in 10" />
       </div>

   </div>
</template>

<script>
  import NavBar from "./components/NavBar.vue"
 import Caroussel from "./components/Caroussel.vue"
  import TeeShirtCard from "./components/TeeShirtCard.vue"
export default {
  name: 'app',
  components: {
      NavBar,
      Caroussel,
      TeeShirtCard
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
