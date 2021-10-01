<template>
  <footer>
    
    <!-- sezione superiore del footer  -->
    <section class="footer_top">

      <div class="box">

        <section>
          
          <div class="logo_cont">

            <img src="../assets/images/avada-drivers-logo-1x.png" alt="">

          </div>

          <p>
            Avada Driving School is the right choise for 
            experienced drivers looking for a refresher
            course or the brand new driver wanting to
            pass first time.
          </p>

        </section>

        <!-- CONTACT DETAILS  -->
        <section>

          <h1>
            CONTACT DETAILS
          </h1>

          <ul>

            <li v-for="(contactDetail, index) in contactDetails" :key="index">

              <i :class="contactDetail.icon"></i>

              <span>
                {{ contactDetail.text }}
              </span>
               
            </li>

          </ul>

        </section>
        <!-- / CONTACT DETAILS  -->

        <!-- COURSES -->
        <section>

          <h1>
            COURSES
          </h1>

          <ul>

            <li v-for="(course, index) in courses" :key="index">
              <i class="far fa-arrow-alt-circle-right"></i>
              {{ course.text }}
            </li>

          </ul>


        </section>
        <!-- / COURSES -->

        <section>
          
          <div class="discount_cont">

            <img src="../assets/images/footer-ad-grid.png" alt="discount footer grid">

          </div>

          <div class="book_now">
            BOOK NOW
          </div>

        </section>

      </div>

    </section>
    <!-- / sezione superiore del footer  -->

    <!-- sezione inferiore del footer  -->
    <section class="footer_bottom">

      <div class="box">

        <section>

          <p>
            <i class="far fa-copyright"></i> Copyright 2012 - 2020 | Avada Theme by <span>ThemeFusion</span> | All Rights Reserved| Powered by <span>WordPress</span>
          </p>

        </section>

        <section>

          <i class="fab fa-facebook-f"></i>
          <i class="fab fa-twitter"></i>
          <i class="fab fa-youtube"></i>
          <i class="fab fa-instagram"></i>

        </section>
        
      </div>
      
    </section>
    <!-- / sezione inferiore del footer  -->
  </footer>
</template>

<script>
export default {
    name: 'Footer',
    data() {
      return {
        contactDetails: [
          {
            icon: "fas fa-home",
            text: "12345 North Main Street, New York, NY 555555"
          },
          {
            icon: "fas fa-phone",
            text: "1.800.555.6789"
          },
          {
            icon: "fas fa-envelope",
            text: "info@your-domain.com"
          },
          {
            icon: "fas fa-link",
            text: "Theme-Fusion.com"
          },
        ],
        courses: [
          {
            icon: "far fa-arrow-alt-circle-right",
            text: "Pass Plus"
          },
          {
            icon: "far fa-arrow-alt-circle-right",
            text: "Intensive Course"
          },
          {
            icon: "far fa-arrow-alt-circle-right",
            text: "Automatic"
          },
          {
            icon: "far fa-arrow-alt-circle-right",
            text: "Instructor Training"
          },
        ]
      }
    }
}
</script>

<style scoped lang="scss">
@import "../style/generals";
@import "../style/vars";
@import '~@fortawesome/fontawesome-free/css/all.min.css';

.footer_top {
  width: 100%;
  height: 380px;
  // background-color: rgb(55, 0, 255);
  background-image: url("../assets/images/footer-background-color.jpg");
  background-repeat: no-repeat;
  background-size: cover;

  .box section {
    width: calc(100% / 4);
    height: 100%;
    // background-color: rgb(0, 255, 21);
    border: 1px solid black;

    ul li {
      list-style-type: none;
    }

    .discount_cont {
      width: 210px;
      height: 210px;

      img {
        width: 100%;
        height: 100%;
      }
    }
    .book_now {
      width: 50%;
      height: 30px;
      padding: 5px 15px;
      margin-bottom: -20px;
      border-radius: 10px;
      background-color: $lightgreen;
      color: white;
      display: flex;
      justify-content: center;
    }
  }
}
.footer_bottom {
  width: 100%;
  height: 120px;
  // background-color: rgb(55, 0, 255);
  background-color: $footer;

  .box section {
    width: calc(100% / 2);
    height: 100%;
    // background-color: rgb(255, 0, 0);
    // border: 1px solid black;
    display: flex;
    justify-content: flex-end;
    align-items: center;

    p {
      font-size: 11px;
      color: $gray;

      i {
        color: $gray;
      }

      span {
        color: $darklightgreen;
      }
    }

    i {
      margin: 5px;
      color: white;
    }
  }
}
.box {
  width: 75%;
  height: 100%;
  margin: auto;
  // background-color: darkolivegreen;
  display: flex;
}

</style>