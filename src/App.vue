<template>
  <div id="app">
      <myHeader/>

    <section>
      <myJumbotron/>
    </section>

    <main>
      <sectionContent/>
    </main>

    <footer>
      <myFooter/>
    </footer>
  </div>
</template>

<script>
import myHeader from './components/myHeader.vue'
import myJumbotron from './components/myJumbotron.vue'
import myFooter from './components/myFooter.vue'
import sectionContent from './components/sectionContent.vue'

export default {
  name: 'App',
  components: {
    myHeader,
    myJumbotron,
    myFooter,
    sectionContent
}
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Teko:wght@300;400;500;600;700&display=swap');

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

a, h2, h3 {
  font-family: Teko;
}
</style>
