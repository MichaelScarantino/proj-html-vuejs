<template>
  <div id="app">
    <Header :headerArray="headerNavList"/>
    <Main />
    <Footer :footerArray="footerList"/>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer
  },
  data: function() {
    return{
      headerNavList: [
        {
          name: 'home',
          active: true
        },
        {
          name: 'about',
          active: false
        },
        {
          name: 'departments',
          active: false
        },
        {
          name: 'articles',
          active: false
        }
      ],
      footerList: [
        {
          social: [
            {
              tag: '<i class="fab fa-facebook-f"></i>',
              bgrColor: '#3c5998'
            },
            {
              tag: '<i class="fab fa-twitter"></i>',
              bgrColor: '#54acee'
            },
            {
              tag: '<i class="fab fa-youtube"></i>',
              bgrColor: '#cc201f'
            },
            {
              tag: '<i class="fab fa-instagram"></i>',
              bgrColor: '#40729b'
            }
          ]
        },
        {
          medical: [
            {
              name: 'Cardiology'
            },
            {
              name: 'Pediactrics'
            },
            {
              name: 'Diabetes Care'
            },
            {
              name: 'Pre-natel Care'
            },
            {
              name: 'Ultrasound Echocardiogram'
            }
          ]
        }
        
      ],
    };
  },
};
</script>

<style lang="scss">
@import './styles/general.scss';

</style>
