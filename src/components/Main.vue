<template>
  <!-- Main -->
  <main>
    <Welcome />
    <Meet />
    <Services />
    <Facilities />
    <LearnMore />
    <Appointment />
  </main>
</template>

<script>
import Welcome from "../components/Welcome.vue";
import Meet from "../components/Meet.vue";
import Services from "../components/Services.vue";
import Facilities from "../components/Facilities.vue";
import LearnMore from "../components/LearnMore.vue";
import Appointment from "../components/Appointment.vue";

export default {
  name: "Main",
  components: {
    Welcome,
    Meet,
    Services,
    Facilities,
    LearnMore,
    Appointment,
  },
};
</script>

<style scoped lang="scss">

</style>