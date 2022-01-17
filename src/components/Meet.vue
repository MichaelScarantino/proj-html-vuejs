<template>
    <section class="meet">
        <!-- Wrapper -->
        <div class="wrapper">
            <!-- Container Fluid -->
            <div class="container-fluid">
                <!-- Welcome Main Text -->
                <div class="main-text-and-icon">
                    <div class="single-icon">
                        <img src="../assets/images/icon-5.png" alt="Doctor Icon">
                    </div>
                    <h3>meet our doctors</h3>
                    <p>Sed ut perspiciatis unde omnis iste natus error sit valuptatem accusatium doloremque laudatium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architeto beatae.</p>
                </div>
                <!-- Row -->
                <div class="row">
                    <!-- Col -->
                    <div class="col">
                        <!-- Single Doctor -->
                        <div class="single-doctor">
                            <!-- Single Doctor Img -->
                            <div class="single-doctor-img">
                                <img src="../assets/images/doctor-1-200x206.jpg" alt="Jon Snow Img">
                            </div>
                            <!-- Single Doctor Name -->
                            <div class="single-doctor-name">
                                jon snow
                            </div>
                            <!-- Single Doctor Trade -->
                            <div class="single-doctor-trade">
                                Anesthesiologist
                            </div>
                            <!-- Single Doctor Info -->
                            <div class="single-doctor-info">
                                <p>At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque</p> 
                            </div>
                            <!-- Single Social -->
                            <div class="single-social">
                                <ul>
                                    <li class="bgr-facebook">
                                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                                    </li>
                                    <li>
                                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                                    </li>
                                    <li>
                                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                                    </li>
                                </ul>
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
  components: {
  },
};
</script>

<style scoped lang="scss">
.meet{
    background-color: #f7f7f7;
    .single-social{
        ul{
            li{
                display: inline-block;
                margin: 0 20px;
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
</style>