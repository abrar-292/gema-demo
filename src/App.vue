<template>
  <div class="w-100 container-fluid mx-0 px-0">
    <Navbar/>
    <Header/>
    <WhatWeDo/>
    <Idea/>
    <ContactUs/>
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from './components/Navbar'
import Header from './components/Header'
import WhatWeDo from './components/WhatWeDo'
import Idea from './components/Idea'
import 'bootstrap/scss/bootstrap.scss'
import './style.scss'
import Footer from "./components/Footer";
import ContactUs from "./components/ContactUs";


export default {
  name: 'App',
  components: {
    ContactUs,
    Footer,
    Navbar,
    Header,
    WhatWeDo,
    Idea,
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
