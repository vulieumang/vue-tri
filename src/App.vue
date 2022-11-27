<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <Header />
  <main class="flex flex-col justify-center">
    <FormToken />
  </main>
  <Footer />
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import FormToken from './components/FormToken.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    FormToken
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
main {
  min-height: calc(100vh - 134px);
}
</style>
