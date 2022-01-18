<template>
    <!-- Header -->
    <header>
        <!-- Header Top -->
        <section class="header-top">
            <!-- Container -->
            <div class="container-fluid">
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
            <!-- Wrapper -->
            <div class="wrapper">
                <!-- Container Fluid -->
                <div class="container-fluid">
                    <!-- Jumbotron -->
                    <div class="jumbotron">
                        <!-- Jumbotron Title -->
                        <div class="jumbotron-title">
                            <h2>Caring <span class="active">For Life</span></h2>
                        </div>
                        <!-- Jumbotron Cta -->
                        <div class="jumbotron-cta">
                            <!-- Jumbotron Description -->
                            <div class="jumbotron-cta-description">
                                <p>Kind words can be short and easy to speak, but their echoes are truly endless. Avada Health focuses on you as if it was our own family.</p>
                            </div>
                            <!-- Jumbotron Btn -->
                            <div class="jumbotron-cta-btn">
                                <a class="ms_btn ms_btn-lightblue" href="#">learn more</a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
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

// Header
header{
    width: 100%;
    height: 100vh;
    background-image: url('../assets/images/header-image-homepage.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    color: white;
    // Header Top
    .header-top{
        width: 100%;
        padding: 30px;
        text-transform: uppercase;
        font-size: 12px;
        // Header Menu
        &-menu{
            li{
                margin: 0 20px;
            }
        }
    }
    // Header Bottom
    .header-bottom{
        // Jumbotron
        .jumbotron{
            padding: 130px 0;
            width: 70%;
            // Jumbotron Title
            &-title{
                h2{
                    font-size: 55px;
                }
            }
            // Jumbotron Cta
            &-cta{
                // Jumbotron Cta Description
                &-description{
                    padding: 20px 0;
                    color: #d7d0cf;
                    font-size: 18px;
                }
                // Jumbotron Cta Btn
                &-btn{
                    text-transform: uppercase;
                    font-size: 14px;
                }
            }
        }
    }
}
</style>