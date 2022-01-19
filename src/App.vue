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
          socials: [
            {
              class: 'fab fa-facebook-f',
              bgrColor: '#3c5998'
            },
            {
              class: 'fab fa-twitter',
              bgrColor: '#54acee'
            },
            {
              class: 'fab fa-youtube',
              bgrColor: '#cc201f'
            },
            {
              class: 'fab fa-instagram',
              bgrColor: '#40729b'
            }
          ]
        },
        {
          departments: [
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
