<template>
    <!-- Welcome -->
    <section class="Welcome">
        <!-- Wrapper -->
        <div class="wrapper">
            <!-- Container Fluid -->
            <div class="container-fluid">
                <!-- Welcome Main Text -->
                <div class="main-text">
                    <h3>Welcome to Avada Health</h3>
                    <p>Sed ut perspiciatis unde omnis iste natus error sit valuptatem accusatium doloremque laudatium, totam rem aperiam, eaque ipsa quae ab illo.</p>
                </div>
                <!-- Row -->
                <div class="row">
                    <!-- Col -->
                    <div v-for="(welcomeDetail, index) in welcomeDetails" :key="index" class="col">
                        <!-- Single Description -->
                        <div class="single-description">
                            <!-- Single Description Icon -->
                            <div class="single-description-icon">
                                <img :src="require(`../assets/images/${welcomeDetail.image}.png`)" :alt="welcomeDetail.alt">
                            </div>
                            <!-- Single Description Text -->
                            <div class="single-description-text">
                                <h4>{{ welcomeDetail.title }}</h4>
                                <p>{{ welcomeDetail.text }}</p>
                            </div>
                        </div>
                    </div>
                    
                </div>
                <!-- End Row -->
            </div>
        </div>
    </section>
</template>

<script>

export default {
  name: "Welcome",
  props: {
      welcomeDetails:Array
  },
};
</script>

<style scoped lang="scss">

</style>