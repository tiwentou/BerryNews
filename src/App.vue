<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>

export default {
  name: 'app',

}

//<router-link :to="{name: 'home'}">Home</router-link>
//<router-link :to="{name: 'article', params: {id: 1}}">Article 1</router-link>
//<router-link :to="{name: 'article', params: {id: 2}}">Article 2</router-link>
</script>



<style>
html, body, #app {
  width: 100%;
  height: 100%;
}

body {
  margin: 0;
}


#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #CECECE;
}
</style>
