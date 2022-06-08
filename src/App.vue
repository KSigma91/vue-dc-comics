<template>
  <div id="app">
    <myHeader/>
    <calltoAction/>
    <myMain/>
    <myFooter/>
  </div>
</template>

<script>
import myHeader from './components/myHeader.vue'
import calltoAction from './components/calltoAction.vue'
import myMain from './components/myMain'
import myFooter from './components/myFooter'

export default {
  name: 'App',
  components: {
    myHeader,
    calltoAction,
    myMain,
    myFooter
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
