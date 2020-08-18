<template>
  <div id="app">
    <header>
      <HeaderComponent/>
    </header>
    
    <HelloWorld msg="It's working!!"/>

    <footer>
      <FooterComponent/>
    </footer>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import HeaderComponent from './components/HeaderComponent.vue'
import FooterComponent from './components/FooterComponent.vue'

export default {
  name: 'App',
  components: {
    'HelloWorld': HelloWorld,
    'HeaderComponent': HeaderComponent,
    'FooterComponent': FooterComponent
  }
}
</script>

<style>
#app {
  font-family: Palatino, Palatino Linotype, Palatino LT STD, Book Antiqua, Georgia, serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
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