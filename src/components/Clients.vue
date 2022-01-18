<template>
  <!-- Clients -->
  <div class="clients">
    <!-- Wrapper -->
    <div class="wrapper">
      <!-- Container Fluid -->
      <div class="container-fluid">
        <!-- Clients Logo -->
        <div class="clients-logo">
            <img class="client-logo" src="../assets/images/client-logos-1-200x188.png" alt="Healthy Logo">
            <img class="client-logo" src="../assets/images/client-logos-2-200x188.png" alt="Healt Logo">
            <img class="client-logo" src="../assets/images/client-logos-3-200x188.png" alt="Turbo Power Logo">
            <img class="client-logo" src="../assets/images/client-logos-4-200x188.png" alt="Color People Logo">
        </div>
        
      </div>
    </div>
    
    
  </div>
</template>

<script>


export default {
  name: "Clients",
};
</script>

<style scoped lang="scss">

// Clients
.clients{
  background-image: url('../assets/images/rgb-gradient-bar-for-logo-carrasel.jpg');
  background-size: cover;
  background-repeat: no-repeat;
  // Wrapper
  .wrapper{
    overflow: hidden;
    // Clients Logo
    .clients-logo{
      padding: 30px 0;
      // Client Logo
      .client-logo{
        position: relative;
        top: 0;
        left: -800px;
        animation: sponsor-slide 5s linear infinite;
      }
      @keyframes sponsor-slide {
        100% {transform: translate(1600px);}
      }
    }
  }
}
</style>