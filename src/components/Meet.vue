<template>
    <!-- Meet -->
    <section class="meet">
        <!-- Wrapper -->
        <div class="wrapper">
            <!-- Container Fluid -->
            <div class="container-fluid">
                <!-- Meet Main Text and Icon -->
                <div class="main-text-and-icon">
                    <!-- Single Icon -->
                    <div class="single-icon">
                        <img src="../assets/images/icon-5.png" alt="Doctor Icon">
                    </div>
                    <h3>meet our doctors</h3>
                    <p>Sed ut perspiciatis unde omnis iste natus error sit valuptatem accusatium doloremque laudatium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architeto beatae.</p>
                </div>
                <!-- Row -->
                <div class="row">
                    <!-- Col -->
                    <div v-for="(meetDetail, index) in meetDetails" :key="index" class="col">
                        <!-- Single Doctor -->
                        <div class="single-doctor">
                            <!-- Single Doctor Img -->
                            <div class="single-doctor-img">
                                <img :src="require(`../assets/images/${meetDetail.image}.jpg`)" alt="Jon Snow Img">
                            </div>
                            <div class="single-doctor-info">
                                <!-- Single Doctor Name -->
                                <div class="single-doctor-name">
                                    {{ meetDetail.name }}
                                </div>
                                <!-- Single Doctor Trade -->
                                <div class="single-doctor-trade">
                                    {{ meetDetail.trade }}
                                </div>
                                <!-- Single Doctor Info -->
                                <div class="single-doctor-description">
                                    <p>{{ meetDetail.description }}</p> 
                                </div>
                                <!-- Single Doctor Social -->
                                <div class="single-doctor-social">
                                    <ul>
                                        <li class="bgr-facebook">
                                            <a href="#"><i class="fab fa-facebook-f"></i></a>
                                        </li>
                                        <li class="bgr-twitter">
                                            <a href="#"><i class="fab fa-twitter"></i></a>
                                        </li>
                                        <li class="bgr-instagram">
                                            <a href="#"><i class="fab fa-instagram"></i></a>
                                        </li>
                                    </ul>
                                </div>
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
  name: "Main",
  props: {
      meetDetails: Array
  },
};
</script>

<style scoped lang="scss">
// Meet
.meet{
    background-color: #f7f7f7;
    // Single Doctor
    .single-doctor{
        margin: 0 5px;
        background-color: white;
        // Single Doctor img
        &-img{
            width: 100%;
            img{
                width: 100%;
            }
        }
        // Single Doctor info
        .single-doctor-info{
            padding: 20px;
            // Single Doctor name
            .single-doctor-name{
                text-transform: uppercase;
            }
            // Single Doctor trade
            .single-doctor-trade{
                font-size: 13px;
            }
            // Single Doctor Description
            .single-doctor-description{
                font-size: 12px;
                color: gray;
                padding: 20px 0;
            }
            // Single Doctor Social
            .single-doctor-social{
                ul{
                    margin-left: -5px;
                    li{
                        display: inline-block;
                        margin: 0 5px;
                        color: white;
                        width: 30px;
                        height: 30px;
                        text-align: center;
                        position: relative;
                        border-radius: 3px;
                        i{
                            position: absolute;
                            top: 50%;
                            left: 50%;
                            transform: translate(-50%, -50%);
                        }
                    }
                }
            }
        }
    }
    
}
</style>