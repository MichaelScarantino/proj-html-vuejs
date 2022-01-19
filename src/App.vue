<template>
  <div id="app">
    <Header :headerArray="headerNavList"/>
    <Main :welcomeArray="mainWelcomeList" :meetArray="mainMeetList" :servicesArray="mainServicesList" />
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
      mainWelcomeList: [
        {
          image: 'icon-1',
          alt: 'Phone icon',
          title: 'same day appointmants',
          text: 'Sed ut perspicatis unde omnis iste natus error sit voluptam accusatim'
        },
        {
          image: 'icon-2',
          alt: 'Bed icon',
          title: 'world class facilities',
          text: 'Sed ut perspicatis unde omnis iste natus error sit voluptam accusatim'
        },
        {
          image: 'icon-3',
          alt: 'Head icon',
          title: 'expert doctors',
          text: 'Sed ut perspicatis unde omnis iste natus error sit voluptam accusatim'
        },
        {
          image: 'icon-4',
          alt: 'Microscope icon',
          title: 'complementary therapies',
          text: 'Sed ut perspicatis unde omnis iste natus error sit voluptam accusatim'
        },
      ],
      mainMeetList: [
        {
          image: 'doctor-1-200x206',
          name: 'jon snow',
          trade: 'Anesthesiologist',
          description: 'At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque',
        },
        {
          image: 'doctor-2-200x206',
          name: 'tony stark',
          trade: 'Cardiologist',
          description: 'At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque',
        },
        {
          image: 'doctor-3-200x206',
          name: 'anna smith',
          trade: 'Nurse praticatitioner',
          description: 'At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque',
        }
      ],
      mainServicesList: [
        {
          image: 'icon-14',
          alt: 'Ambulance Icon',
          title: 'rehabilitation center',
          text: 'At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditis praesentium voluptatitum deleniti atque corrupti quos dolores et quas'
        },
        {
          image: 'icon-15',
          alt: 'Tooth Icon',
          title: 'dental implants',
          text: 'At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditis praesentium voluptatitum deleniti atque corrupti quos dolores et quas'
        },
        {
          image: 'icon-16',
          alt: 'Chemical Container Icon',
          title: 'medicine research',
          text: 'At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditis praesentium voluptatitum deleniti atque corrupti quos dolores et quas'
        },
        {
          image: 'icon-11',
          alt: 'Drip Icon',
          title: 'blood bank',
          text: 'At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditis praesentium voluptatitum deleniti atque corrupti quos dolores et quas'
        },
        {
          image: 'icon-12',
          alt: 'Medicinal Icon',
          title: 'pharmaceutical advice',
          text: 'At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditis praesentium voluptatitum deleniti atque corrupti quos dolores et quas'
        },
        {
          image: 'icon-13',
          alt: 'Medical Instrument Icon',
          title: 'medical counseling',
          text: 'At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditis praesentium voluptatitum deleniti atque corrupti quos dolores et quas'
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
