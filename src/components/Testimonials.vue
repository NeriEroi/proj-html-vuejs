<template>
  <!-- TESTIMONIALS  -->
  <section class="testimonials">

    <div class="title_p_cont">
      <div class="title_cont">
        <h1>
          Testimonials
        </h1>
      </div>
      <p>
        Here's what our happy drivers hat to say about our services:
      </p>
    </div>

    <div class="image_cont">
      <img src="../assets/images/testimonial-sophia.png" alt="testimonial sophia jones">
    </div>

    <div class="text_cont">
      
      Avada Driving School really helped build my confidence behind the 
      wheel and with driving in general, and they got me a first time pass!
      <p>Highly recommended</p>
      
    </div>

    <div class="signature_cont">
      <h4>
        Sophia Jones
      </h4>
    </div>

    <div class="small_circles_cont">

      <div class="circle fill">

      </div>

      <div class="circle">

      </div>

      <div class="circle">
        
      </div>

      <div class="circle">
        
      </div>

      <div class="circle">
        
      </div>

    </div>        

  </section>
  <!-- / TESTIMONIALS  -->
</template>

<script>
export default {
  name: 'Testimonials',
}
</script>

<style scoped lang="scss">
@import "../style/generals";
@import "../style/vars";
@import '~@fortawesome/fontawesome-free/css/all.min.css';

// TESTIMONIALS
.testimonials {
  width: 100%;
  height: 650px;
  background-image: url("../assets/images/testimonial-background.jpg");
  background-size: cover;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  .title_p_cont .title_cont {
    display: flex;
    justify-content: center;
    color: $footer;
    margin-top: 50px;
  }

  .title_p_cont {
    color: $gray;
    margin-bottom: 40px;
  }

  .image_cont {
    width: 100px;
    height: 100px;
    margin-bottom: 40px;

    img {
      width: 100%;
      height: 100%;
    }
  }

  .text_cont {
    color: $gray;
    width: 35%;
    text-align: center;

    p {
      text-align: center;
      color: $gray;
    }
  }
  
  .signature_cont {
    padding: 20px 50px;
    color: $gray;
  }

  .small_circles_cont {
    display: flex;

    .circle.fill {
      width: 10px;
      height: 10px;
      border-radius: 50%;
      background-color: $gray;
    }

    .circle {
      width: 10px;
      height: 10px;
      border-radius: 50%;
      border: 3px solid $gray;
      margin: 5px;
    }
  }
}
// / TESTIMONIALS
</style>