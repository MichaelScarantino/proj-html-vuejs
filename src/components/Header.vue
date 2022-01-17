<template>
<!-- Header -->
    <header>
        <!-- Header Top -->
        <section class="header-top">
            <!-- Container -->
            <div class="container">
                <!-- Row -->
                <div class="row align-items-center">
                    <!-- Col -->
                    <div class="col-2">
                        <!-- Header Logo -->
                        <div class="header-top-logo">
                            <img src="../assets/images/medical_logo_1x_light.png" alt="">
                        </div>
                    </div>
                    <!-- Col -->
                    <div class="col flex-grow-1">
                        <!-- Header Menu -->
                        <nav class="header-top-menu d-flex justify-content-end">
                            <ul class="d-flex ">
                                <li v-for="(headerElement, index) in headerArray" :key="index" :class="{'active': headerElement.active}">
                                    <a href="#">{{ headerElement.name }}</a>
                                </li>
                            </ul>
                        </nav>
                    </div>
                    <!-- Col -->
                    <div class="col-2">
                        <!-- Header Appointment -->
                        <div class="header-top-appointment d-flex justify-content-center">
                            <a class="ms_btn ms_btn-lightblue" href="#">make appointment</a>
                        </div>
                    </div>
                </div>
                <!-- End Row -->
            </div>
        </section>

        <!-- Header Bottom -->
        <section class="header-bottom">

        </section>
    </header>
</template>

<script>

export default {
  name: "Header",
  components: {
  },
  props: {
      headerArray: Array
  }
};
</script>

<style scoped lang="scss">
@import '../styles/variables.scss';
header{
    width: 100%;
    background-image: url('../assets/images/header-image-homepage.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    color: white;

    // TEST
    height: 400px;

    .header-top{
        width: 100%;
        padding: 20px 0;
        text-transform: uppercase;
        font-size: 14px;

        .header-top-menu{
            li{
                margin: 0 20px;
            }
        }
    }
}
</style>