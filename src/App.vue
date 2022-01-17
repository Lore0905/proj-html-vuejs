<template>
  <div id="app">
    <header>
      <Header :links="headerLinks"/>
    </header>
    <main>
      <Main/>
    </main>
    <footer>
      <Footer/>
    </footer>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  },
  data: function(){
    return{
      headerLinks: [
        {
          title: 'HOME',
          href: '#'
        },
        {
          title: 'ABOUT',
          href: '#'
        },
        {
          title: 'SERVICES',
          href: '#'
        },
        {
          title: 'PRICING',
          href: '#'
        },
        {
          title: 'BLOG',
          href: '#'
        }
      ]
    }
  }
}
</script>

<style lang="scss">
@import './style/variables.scss';
@import './style/general.scss';
@import './style/common.scss';

footer{
  border: 1px solid black;
}

</style>
