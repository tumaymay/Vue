<template>
  <div id="app">
    <img src="./assets/logo.png" />
    
   

    <Big/>

  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import MyComponent from './components/myComponent'
import Parent from './components/sonparent/parent'
import Parents from './components/slots/parent'
import Big from './components/comkeep/big'


export default {
  name: 'App',
  components: {
    HelloWorld,
    MyComponent,
    Parent,
    Parents,
    Big
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
