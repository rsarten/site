<template>
  <div id="app">
    <header>
      <Header/>
    </header>
    
    <Body/>

    <footer>
      <Footer/>
    </footer>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Body from './components/Body.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    'Header': Header,
    'Body': Body,
    'Footer': Footer
  }
}
</script>

<style>
#app {
  font-family: Palatino, Palatino Linotype, Palatino LT STD, Book Antiqua, Georgia, serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /*text-align: left;
  color: #2c3e50;
  margin-top: 60px;*/
  width: 100%;
}

header, footer {
  padding: 1em;
  color: white;
  background-color: #2d3d56;
  clear: left;
  text-align: center;
  border-radius: 4px;
}

</style>