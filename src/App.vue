<template>
  <v-app>
    <Header/>
    <Info />
    <Footer/>
  </v-app>
</template>

<script>
import Header from './components/Header'
import Info from './components/Info'
import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    Header,
    Info,
    Footer
  }
}
</script>

<style>
  #app {
    font-family: Arial, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    background-color: #F0F4C3;
    box-sizing: border-box;
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    outline: none;
    display: flex;
    flex-flow: column nowrap;
  }

  html, body {
    height: 100%;
    width: 100%;
    padding: 0;
    margin: 0;
  }

  a {
    color: #356859 !important;
    text-decoration: none;
  }

  .fade-enter-active,
  .fade-leave-active {
    transition-duration: 0.3s;
    transition-property: opacity;
    transition-timing-function: ease;
  }

  .fade-enter,
  .fade-leave-active {
    opacity: 0
  }

  html::-webkit-scrollbar-track
  {
    background-color: #FFFFFF;
  }
  html::-webkit-scrollbar
  {
    width: 10px;
    background-color: #F5F5F5;
  }
  html::-webkit-scrollbar-thumb
  {
    background-color: #2E7D32;
  }
  html::-webkit-scrollbar-thumb:hover
  {
    background-color: #1B5E20;
  }
</style>