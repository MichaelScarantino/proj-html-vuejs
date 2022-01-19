<template>
  <!-- Footer -->
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
                <!-- Footer Avada Logo -->
                <div class="footer-avada-logo">
                  <img src="../assets/images/medical_logo_1x_dark.png" alt="Avada Logo">
                </div>
                <!-- Footer Avada Text -->
                <div class="footer-avada-text">
                  <p>Sed ut perspiciatis unde omnis iste natus error sit valuptatem accusatium doloremque laudatium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architeto beatae luptatem accusantium, remaperiamsiat. Voluptatem accusest etsium doloremque laudaien. Lorem ipsum sits dolores ets unser.</p>
                  <h6>learn more about us</h6>
                </div>
              </div>
              <!-- Col -->
              <div class="col">
                <!-- Footer Social List -->
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
          <!-- Footer Contact -->
          <div class="footer-contact">
            <h6>contact information</h6>
            <!-- Contact List -->
            <div class="footer-contact-list">
              <ul>
                <li>
                  <a href="#"><span class="contact-icon"><i class="fas fa-map-marker-alt"></i></span> 121 King Street, London United Kingdom</a>
                </li>
                <li>
                  <a href="#"><span class="contact-icon"><i class="fas fa-phone"></i></span> 1.800.458.556</a>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="col">
          <!-- Footer Medical Department -->
          <div class="footer-medical-department">
            <h6>medical departments</h6>
            <!-- Department List -->
            <div class="footer-department-list">
              <ul>
                <li v-for="(department, index) in footerArray[1].departments" :key="index">
                  <a href="#"><span class="arrow"><i class="fas fa-chevron-right"></i></span>{{ department.name }}</a>
                </li>
              </ul>
            </div>
            <!-- Footer Department Button -->
            <div class="footer-department-button">
              <a class="ms_btn ms_btn-dark" href="#">view our departments</a>
            </div>
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
@import '../styles/variables.scss';

// Footer
footer{
  padding: 40px 30px;
  margin-bottom: 50px;
  font-size: 12px;
  color: gray;
  h6{
        text-transform: uppercase;
        margin-top: 5px;
        color: black;
      }
      // Avada Social Footer
  .avada-and-social-footer{
    // Footer Avada Logo
    .footer-avada-logo{
      img{
        width: 50%;
      }
    }
    // Footer Avada Text
    .footer-avada-text{
      p{
        padding: 15px 0;
        border-bottom: 1px solid lightgray;
        margin-right: 10px;
      }
      h6{
        color: gray;
      }
    }
    // Footer Social List
    .footer-social-list{
      ul{
        margin-left: -5px;
        margin-top: 15px;
        li{
          display: inline-block;
          margin: 0 5px;
          color: white;
          width: 25px;
          height: 25px;
          position: relative;
          border-radius: 3px;
        }
      }
    }
  }
  // Footer Contact
  .footer-contact{
    // Footer Contact List
    .footer-contact-list{
      li{
        padding-bottom: 10px;
        // Contact Icon
        .contact-icon{
          color: $primary_color;
          margin-right: 10px;
        }
      }
    }
  }
  // Commons Footer Contact and Footer Medical Department
  .footer-contact,
  .footer-medical-department{
    h6{
      &::after{
        content: '';
        width: 30px;
        height: 1px;
        display: block;
        margin: 20px 0;
        background-color: $primary_color;
      }
    }
  }
  // Footer Medical Department
  .footer-medical-department{
    // Footer Department List
    .footer-department-list{
      li{
        margin-bottom: 5px;
        // Arrow
        .arrow{
          width: 20px;
          height: 20px;
          border-radius: 100%;
          display: inline-block;
          background-color: $primary_color;
          position: relative;
          color: white;
          vertical-align: middle;
          margin-right: 10px;
        }
      }
    }
    // Footer Department Button
    .footer-department-button{
      text-transform: uppercase;
      font-size: 16px;
      margin-top: 45px;
    }
  }
  // Commons Footer Social List and Footer Medical Department
  .footer-social-list,
  .footer-medical-department{
    i{
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }
  }
}
</style>