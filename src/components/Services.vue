<template>
    <!-- Services -->
    <section class="services">
        <!-- Wrapper -->
        <div class="wrapper">
            <!-- Container Fluid -->
            <div class="container-fluid">
                <!-- Services Main Text and Icon -->
                <div class="main-text-and-icon">
                    <!-- Single Icon -->
                    <div class="single-icon">
                        <img src="../assets/images/icon-6.png" alt="Heart Icon">
                    </div>
                    <h3>our health services</h3>
                    <p>Sed ut perspiciatis unde omnis iste natus error sit valuptatem accusatium doloremque laudatium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architeto beatae.</p>
                </div>
                <!-- Row -->
                <div class="row row-cols-3">
                    <!-- Col -->
                    <div v-for="(serviceDetail, index) in servicesDetails" :key="index" class="col">
                        <!-- Single Description -->
                        <div class="single-description">
                            <!-- Single Description Icon -->
                            <div class="single-description-icon">
                                <img :src="require(`../assets/images/${serviceDetail.image}.png`)" :alt="serviceDetail.alt">
                            </div>
                            <!-- Single Description Text -->
                            <div class="single-description-text">
                                <h4>{{ serviceDetail.title }}</h4>
                                <p>{{ serviceDetail.text }}</p>
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
  name: "Services",
  props: {
      servicesDetails: Array
  }
};
</script>

<style scoped lang="scss">
// Single Description
.single-description{
    margin: 25px 0;
}
</style>