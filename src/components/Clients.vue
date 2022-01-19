<template>
  <!-- Clients -->
  <div class="clients">
    <!-- Wrapper -->
    <div class="wrapper">
      <!-- Container Fluid -->
      <div class="container-fluid">
        <!-- Clients Logo -->
        <div class="clients-logo">
          <img class="client-logo" src="../assets/images/client-logos-3-200x188.png" alt="Turbo Power Logo">
          <img class="client-logo" src="../assets/images/client-logos-1-200x188.png" alt="Healthy Logo">
          <img class="client-logo" src="../assets/images/client-logos-4-200x188.png" alt="Color People Logo">
          <img class="client-logo" src="../assets/images/client-logos-3-200x188.png" alt="Turbo Power Logo">
          <img class="client-logo" src="../assets/images/client-logos-2-200x188.png" alt="Healt Logo">
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
    .clients-logo{
      display: flex;
      margin-left: -125px;
      .client-logo{
        padding: 8px;
      }
    }
  }
}
</style>