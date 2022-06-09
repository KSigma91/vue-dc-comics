<template>
  <div id="app">
      <myHeader/>

    <section>
      <myJumbotron/>
    </section>

    <section>
      <sectionContent/>
    </section>
    
    <main>
      <myMain/>
    </main>

    <footer>
      <myFooter/>
    </footer>
  </div>
</template>

<script>
import myHeader from './components/myHeader.vue'
import myJumbotron from './components/myJumbotron.vue'
import myMain from './components/myMain'
import myFooter from './components/myFooter'
import sectionContent from './components/sectionContent.vue'

export default {
  name: 'App',
  components: {
    myHeader,
    myJumbotron,
    myMain,
    myFooter,
    sectionContent
}
}
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  margin: 0 auto;
}
</style>
