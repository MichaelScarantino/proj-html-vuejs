<template>
    <!-- Appointment -->
    <section class="appointment">
        <!-- Wrapper -->
        <div class="wrapper">
            <!-- Container Fluid -->
            <div class="container-fluid">
                <!-- Appointment Main Text -->
                <div class="main-text">
                    <h3>Make An Appointment</h3>
                    <p>Sed ut perspiciatis unde omnis iste natus error sit valuptatem accusatium doloremque laudatium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architeto beatae.</p>
                     <!-- Appointment Form -->
                <div class="appointment-form">
                    <form>
                        <input class="name" type="text" placeholder="Name*">
                        <input class="email" type="email" placeholder="Email*">
                        <input class="phone" type="text" placeholder="Phone Number">
                        <div class="date">
                            <input class="input-date" type="text" placeholder="Appointment Date">
                            <i class="fas fa-calendar-alt"></i>
                        </div>
                        <textarea cols="30" rows="3" placeholder="How can we help?*"></textarea>
                        <input class="ms_btn ms_btn-lightblue submit" type="submit" value="make an appointment">
                    </form>
                </div>
                </div>
               
            </div>    
        </div>
    </section>
</template>

<script>

export default {
  name: "Appointment",
};
</script>

<style scoped lang="scss">
// Appointment
.appointment{
    color: white;
    background-image: url('../assets/images/make-an-appointment.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    // Main Text
    .main-text{
        margin: 40px auto;
        p{
            padding-bottom: 20px;
        }
        h3{
            &::after{
                content: '';
                width: 180px;
                height: 1px;
                display: block;
                background-color: lightgray;
                margin: 20px auto;
            }
        }
        // Appointment Form
        form{
            display: flex;
            flex-wrap: wrap;
            .name,
            .email,
            .phone,
            .date{
                width: calc((100% / 2) - 20px);
                margin: 10px;
            }
            .name,
            .email,
            .phone,
            .input-date,
            textarea{
                padding: 5px 10px;
                background-color: rgba(255, 255, 255, 0);
                border: 1px solid gray;
                color: white;
            }
            .input-date{
                width: 100%;
                height: 100%;
                padding: 0 30px;
            }
            .date{
                position: relative;
            }
            i{
                position: absolute;
                top: 15px;
                left: 10px;
                font-size: 11px;
                color: gray;
            }
            textarea,
            .submit{
                width: 100%;
                margin: 10px;
            }
            .submit{
                border: none;
                text-transform: uppercase;
            }
            input::placeholder,
            textarea::placeholder{
                font-size: 11px;
            }
        }
    }
}

</style>