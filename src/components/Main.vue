<template>
    <main>
        <Welcome />
        <Meet />
    </main>
</template>

<script>
import Welcome from "../components/Welcome.vue";
import Meet from "../components/Meet.vue";

export default {
  name: "Main",
  components: {
    Welcome,
    Meet,
  },
};
</script>

<style scoped lang="scss">

</style>