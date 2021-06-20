<template>
<div id="app">
    <div class ="menu">
      <a v-for="(menuname, i) in menus" :key="i">{{menuname}}</a>

    </div>



    <div v-for="(item, i) in products" :key="i">
      <h4>{{item[0]}}</h4>
      <p>{{item[1]}}</p>
    </div>

 </div>

</template>

<script>

export default {
  name: 'App',
  data(){
    return {
      menus : ['Home', 'Shop', 'About'],
      products : [['역삼동원룸', 80 +' 만원'], ['천호동원룸', 60+' 만원'], ['마포구원룸', 90 +' 만원']],
    }
  },
  components: {
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
}
.menu {
  background: darkslateblue;
  padding: 15px;
  border-radius: 5px;
}
.menu a {
  color: white;
  padding: 10px;
}
</style>
