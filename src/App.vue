<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'

export default {
  name:'App',
  components: {
    Header,
    Main,
    Footer,
    FontAwesomeIcon,

  }

}
</script>

<template>
  <Header />
  <Main />
  <Footer />

</template>

<style lang="scss">

@use './scss/main.scss';



</style>
