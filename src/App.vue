<template>
  <div id="app">
    <AppHeader/>
    <!--<AppBody/>-->
    <AppFooter/>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader'
import AppBody from './components/AppBody'
import AppFooter from './components/AppFooter'

export default {
  name: 'App',
  components: {AppFooter, AppBody, AppHeader}
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
