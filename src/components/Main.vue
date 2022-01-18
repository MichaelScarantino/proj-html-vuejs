<template>
  <!-- Main -->
  <main>
    <Welcome />
    <Meet />
    <Services />
    <Facilities />
  </main>
</template>

<script>
import Welcome from "../components/Welcome.vue";
import Meet from "../components/Meet.vue";
import Services from "../components/Services.vue";
import Facilities from "../components/Facilities.vue";

export default {
  name: "Main",
  components: {
    Welcome,
    Meet,
    Services,
    Facilities,

  },
};
</script>

<style scoped lang="scss">

</style>