<template>
<!-- Learn More -->
    <div class="learn-more">
        <!-- Single Learn More -->
        <div id="emergency" class="single-learn-more">
            <h5>Emergency Care</h5>
            <!-- Single Icon -->
            <div class="single-icon">
                <img src="../assets/images/wave-divider.png" alt="Wave Icon">
            </div>
            <p>Sed ut perspiciatis unde omnis iste natus error sit valuptatem accusatium doloremque laudatium, totam rem aperiam, eaque</p>
            <!-- Learn More Btn -->
            <div class="learn-more-btn">
                <a class="ms_btn ms_btn-white" href="#">learn more</a>
            </div>
        </div>
    
        <!-- Single Learn More -->
        <div id="diagnostics" class="single-learn-more">
            <h5>Expert Diagnostics</h5>
            <!-- Single Icon -->
            <div class="single-icon">
                <img src="../assets/images/wave-divider.png" alt="Wave Icon">
            </div>
            <p>Sed ut perspiciatis unde omnis iste natus error sit valuptatem accusatium doloremque laudatium, totam rem aperiam, eaque</p>
            <!-- Learn More Btn -->
            <div class="learn-more-btn">
                <a class="ms_btn ms_btn-white" href="#">learn more</a>
            </div>
        </div>
    
        <!-- Single Learn More -->
        <div id="rehabilitation" class="single-learn-more">
            <h5>Superb Rehabilitation</h5>
            <!-- Single Icon -->
            <div class="single-icon">
                <img src="../assets/images/wave-divider.png" alt="Wave Icon">
            </div>
            <p>Sed ut perspiciatis unde omnis iste natus error sit valuptatem accusatium doloremque laudatium, totam rem aperiam, eaque</p>
            <!-- Learn More Btn -->
            <div class="learn-more-btn">
                <a class="ms_btn ms_btn-white" href="#">learn more</a>
            </div>
        </div>
    </div>
</template>

<script>


export default {
  name: "LearnMore",
};
</script>

<style scoped lang="scss">
// Import Variables.scss
@import '../styles/variables.scss';

// Learn More
.learn-more{
    color: white;
    display: flex;
    // Single Learn More
    .single-learn-more{
        text-align: center;
        padding: 40px 20px;
        h5{
            font-size: 14px;
        }
        p{
            padding-bottom: 20px;
            font-size: 12px;
        }
        // Single Icon
        .single-icon{
            padding: 0;
        }
        // Learn More Btn
        .learn-more-btn{
            text-transform: uppercase;
            font-size: 12px;
        }
    }
    // Emergency Id
    #emergency{
        background-color: $primary_color;
    }
    // Diagnostics Id
    #diagnostics{
        background-color: #3697c3;
    }
    // Rehabilitation Id
    #rehabilitation{
        background-color: #327ec7;
    }
}
</style>