<template>
  <footer>
    <!-- Container Fluid -->
    <div class="container-fluid">
      <!-- Row -->
      <div class="row row-cols-3">
        <!-- Col -->
        <div class="col">
          <!-- Avada and social Footer -->
          <div class="avada-and-social-footer">
            <!-- Row -->
            <div class="row row-cols-1">
              <!-- Col -->
              <div class="col">
                <div class="footer-avada-logo">
                  <img src="../assets/images/medical_logo_1x_dark.png" alt="">
                </div>
                <div class="footer-avada-text">
                  <p>Sed ut perspiciatis unde omnis iste natus error sit valuptatem accusatium doloremque laudatium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architeto beatae luptatem accusantium, remaperiamsiat. Voluptatem accusest etsium doloremque laudaien. Lorem ipsum sits dolores ets unser.</p>
                  <h6>learn more about us</h6>
                </div>
              </div>
              <!-- Col -->
              <div class="col">
                <div class="footer-social-list">
                  <ul>
                    <li v-for="(social, index) in footerArray[0].socials" :key="index" :style="`background-color : ${social.bgrColor}`">
                      <a href="#"><i :class="`${social.class}`"></i></a>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col">
          <!-- Contact Footer -->
          <div class="contact-footer">
            contact
          </div>
        </div>
        <div class="col">
          <!-- Medical Department Footer -->
          <div class="medical-department-footer">
            medical
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>

export default {
  name: "Footer",
  components: {
  },
  props: {
      footerArray: Array
  }
};
</script>

<style scoped lang="scss">
// Footer
footer{
  padding: 40px 30px;
  font-size: 12px;
  color: gray;
  .avada-and-social-footer{
    .footer-logo{
      width: 50%;
    }
    .footer-avada-text{
      
      p{
        padding: 15px 0;
        border-bottom: 1px solid lightgray;
      }
      h6{
        text-transform: uppercase;
        margin-top: 5px;
      }
    }
    .footer-social-list{
      ul{
        margin-left: -37px;
        margin-top: 30px;
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
</style>