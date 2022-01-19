<template>
    <!-- Facilities -->
    <section class="facilities">
        <!-- Wrapper -->
        <div class="wrapper">
            <!-- Container Fluid -->
            <div class="container-fluid">
                <!-- Facilities Main Text and Icon -->
                <div class="main-text-and-icon">
                    <!-- Single Icon -->
                    <div class="single-icon">
                        <img src="../assets/images/icon-7.png" alt="Eye Icon">
                    </div>
                    <h3>tour our facilities</h3>
                    <p>Sed ut perspiciatis unde omnis iste natus error sit valuptatem accusatium doloremque laudatium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architeto beatae.</p>
                    <!-- Single Icon -->
                    <div class="single-icon">
                        <img class="play" src="../assets/images/play-icon.png" alt="Play Icon">
                    </div>
                </div>
            </div>    
        </div>
    </section>
</template>

<script>

export default {
  name: "Facilities",
};
</script>

<style scoped lang="scss">
// Facilities
.facilities{
    color: white;
    background-image: url('../assets/images/paralax-bg-tour-facilities.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    // Main Text and Icon
    .main-text-and-icon{
        padding: 0;
        margin-top: 60px;
        margin-bottom: 60px;
        p{
            padding-bottom: 20px;
        }
        // Play
        .play{
            cursor: pointer;
        }
    }
}

</style>