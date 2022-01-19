<template>
  <!-- Main -->
  <main>
    <Welcome :welcomeDetails="welcomeArray"/>
    <Meet :meetDetails="meetArray" />
    <Services :servicesDetails="servicesArray" />
    <Facilities />
    <LearnMore />
    <Appointment />
    <Clients />
  </main>
</template>

<script>
import Welcome from "../components/Welcome.vue";
import Meet from "../components/Meet.vue";
import Services from "../components/Services.vue";
import Facilities from "../components/Facilities.vue";
import LearnMore from "../components/LearnMore.vue";
import Appointment from "../components/Appointment.vue";
import Clients from "./Clients.vue";

export default {
  name: "Main",
  components: {
    Welcome,
    Meet,
    Services,
    Facilities,
    LearnMore,
    Appointment,
    Clients,
  },
  props: {
    welcomeArray: Array,
    meetArray: Array,
    servicesArray: Array
  }
};
</script>

<style scoped lang="scss">

</style>