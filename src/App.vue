<template>
  <img alt="logo" src="./assets/BinaryGolayCode.png" id="logo">
  <Title />
  <Matlab />
  <Footer />
</template>

<script>
import Title from './components/Title.vue'
import Matlab from './components/Matlab.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Title,
    Matlab,
    Footer
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

#logo {
  width: 80%;
  max-width: 40rem;
}
</style>
