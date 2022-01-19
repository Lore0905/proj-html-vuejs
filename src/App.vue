<template>
  <div id="app">
    <header>
      <Header :links="headerLinks"/>
    </header>
    <main>
      <Main/>
    </main>
    <footer>
      <Footer :links="footerLinks"/>
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
      ],
      footerLinks: [
        {
          title: 'About',
          link: [
            'The company',
            'Istitutional',
            'Social & Events',
            'Innovation',
            'Environment',
            'Technology',
            
          ]
        },
        {
          title: 'Services',
          link: [
            'Audit & Assurance',
            'Financial Advisory',
            'Analytics M&A',
            'Middle Marketing',
            'Legal Consulting',
            'Regultory Risk',
            
          ]
        },
        {
          title: 'Support',
          link: [
            'Responsibility',
            'Terms of Use',
            'About Cookies',
            'Privacy Policy',
            'Accessibility',
            'Information',
            
          ]
        },
      ]

    }
  }
}
</script>

<style lang="scss">
@import './style/variables.scss';
@import './style/general.scss';
@import './style/common.scss';


</style>
