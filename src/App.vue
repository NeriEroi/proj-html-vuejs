<template>
  <div id="app">

    <Header />

    <main>

      <!-- SECTION REQUEST  -->
      <section class="request">

        <div class="request_wrap">

          <div class="text">

            <div class="text_wrap">

              <h1>
                Get Behind The Wheel
              </h1>

              <p>
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. 
                Quae enim illo quidem eligendi quibusdam laudantium totam iste, dolorem ea, 
                facilis minus modi eum amet pariatur perspiciatis assumenda, mollitia beatae officia!
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. 
                Quae enim illo quidem eligendi quibusdam laudantium totam iste, dolorem ea, 
                facilis minus modi eum amet pariatur perspiciatis assumenda, mollitia beatae officia!
              </p>

            </div>

          </div>

          <div class="form">

            <div class="form_wrap">
              
              <h3>
                First Lesson Free
              </h3>

              <p>
                When you make a block booking with us your first lesson is 
              </p>

              <span>included free</span>

              <input type="text" placeholder="Your Name*">

              <input type="text" placeholder="Email*">

              <input type="text" placeholder="Telephone*">

              <input type="text" placeholder="Location*">

              <div class="button">
                REQUEST A CALLBACK
              </div>

            </div>

          </div>

        </div>

      </section>
      <!-- / SECTION REQUEST  -->

      <!-- SECTION COMMERCIAL  -->
      <section class="commercial">

        <!-- COMMERCIAL TOP  -->
        <div class="commercial_top">

          <div class="commercial_top_wrap">

            <div class="text_wrap">

              <h1>
                Start Learning to Drive Today
              </h1>

              <p>
                Give us a call to schedule your first driving lesson 
              </p>

            </div>

            <div class="number">

              <i class="fas fa-phone"></i>

              <span>1-800-555-555</span>

            </div>

          </div>

        </div>
        <!-- / COMMERCIAL TOP  -->

        <!-- COMMERCIAL BOTTOM  -->
        <div class="commercial_bottom">

          <div class="commercial_bottom_wrap">

            <div class="information_course">

              <div class="triangle">
            
              </div>

              <h3>
                NEW
              </h3>

              <div class="all_info">

                <h2>
                  Courses
                </h2>

                <p>
                  Lorem ipsum dolor sit amet consectetur elit, sit amet consectetur elit. 
                  Voluptatesquis ut reiciendis animi repudiandae in velit?
                </p>

                <div class="button">
                  COURSE INFORMATION
                </div>
              </div>

            </div>

            <div class="learn_more">

              <div class="item">

                <div class="item_square">

                  <img src="./assets/images/courses-passplus-200x200.jpg" alt="courses passplus">

                </div>

                <h5>
                  Pass Plus
                </h5>

                <div class="button">
                  LEARN MORE
                </div>

              </div>

              <div class="item">

                <div class="item_square">

                  <img src="./assets/images/course-intensive-200x200.jpg" alt="course intensive">

                </div>

                <h5>
                  Intensive Course
                </h5>

                <div class="button">
                  LEARN MORE
                </div>

              </div>

              <div class="item">

                <div class="item_square">

                  <img src="./assets/images/courses-instructor-200x200.jpg" alt="courses instructor">

                </div>

                <h5>
                  Instructors
                </h5>

                <div class="button">
                  LEARN MORE
                </div>

              </div>

            </div>

          </div>

        </div>
        <!-- COMMERCIAL BOTTOM  -->

      </section>
      <!-- / SECTION COMMERCIAL  -->
    </main>

    <Footer />
    
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer
  }
}
</script>

<style lang="scss">
@import "./style/generals";
@import "./style/vars";

// SECTION REQUEST 
section.request {
  width: 100%;
  height: 500px;
  margin-bottom: 30px;
  // background-color: green;

  .request_wrap {
    width: 75%;
    height: 100%;
    margin: auto;
    // background-color: rgb(0, 2, 128);
    display: flex;

    .text {
      width: 50%;
      height: 100%;
      // background-color: grey;
      // border: 1px solid black;
      display: flex;
      justify-content: flex-end;
      align-items: center;

      .text_wrap {
        width: 70%;
        height: 70%;
        margin-right: 10px;
        // background-color: rgb(150, 16, 16);
        color: $gray;

        h1 {
          color: $footer;
        }
      }
    }

    .form {
      width: 50%;
      height: 100%;
      // background-color: grey;
      // border: 1px solid black;
      display: flex;
      justify-content: flex-start;
      align-items: center;

      .form_wrap {
        width: 70%;
        height: 100%;
        border-radius: 10px;
        margin-top: -55px;
        margin-left: 10px;
        background-color: white;
        box-shadow: 0px 10px #e7e4e4;
        z-index: 555;
        display: flex;
        flex-direction: column;
        align-items: center;

        h3 {
          margin-top: 25px;
          color: #49963f;
        }

        p {
          margin-top: 25px;
          margin-bottom: 5px;
          font-size: 10px;
          color: $gray;
        }

        span {
          font-size: 10px;
          color: $gray;
        }

        input {
          width: 90%;
          height: 8%;
          padding: 10px;
          margin: 15px;
        }

        .button {
          width: 160px;
          height: 34px;
          border-radius: 20px;
          color: white;
          background-color: #49963f;
          margin-top: 10px;
          font-size: 11px;
          display: flex;
          justify-content: center;
          align-items: center;
          cursor: pointer;
        }
      }
    }
  }
}
// / SECTION REQUEST

// SECTION COMMERCIAL
section.commercial {
  width: 100%;
  height: 500px;
  background-color: lawngreen;
  background-image: url("./assets/images/horizontal-cta-background.jpg");
  background-size: contain;

  .commercial_top {
    width: 100%;
    height: 165px;

    .commercial_top_wrap {
      width: 60%;
      height: 100%;
      margin: auto;
      // background-color: mediumblue;
      display: flex;
      justify-content: space-between;
      align-items: center;

      .text_wrap h1 {
        color: white;
      }

      .text_wrap p {
        color: white;
      }

      .number i {
        color: white;
        margin-right: 30px;
        font-size: 20px;
      }

      .number span {
        color: white;
        margin-right: 150px;
        font-size: 20px;
      }
    }
  }

  .commercial_bottom {
    width: 100%;
    height: 335px;
    // background-color: mediumturquoise;
    background-image: url("./assets/images/promise-background.jpg");
    background-size: 95% 100%;

    .commercial_bottom_wrap {
      width: 60%;
      height: 100%;
      margin: auto;
      // background-color: mediumvioletred;
      display: flex;
      justify-content: space-between;

      .information_course {
        width: 30%;
        height: 80%;
        border-radius: 8px;
        background-color: white;
        position: relative;
        bottom: 5%;

        .triangle {
          width: 0;
          height: 0;
          border-top: 65px solid $darklightgreen;
          border-right: 65px solid transparent;
        }

        h3 {
          transform: rotate(-45deg);
          position: absolute;
          top: 10px;
          left: 3px;
          font-size: 13px;
          color: white;
        }

        .all_info {
          font-size: 15px;
          display: flex;
          flex-direction: column;
          justify-content: center;
          align-items: center;

          h2 {
            margin-top: -20px;
            margin-bottom: 11px;
          }

          p {
            padding: 0 25px 0 25px;
            font-size: 12px;
            text-align: center;
            margin-bottom: 8px;
          }

          .button {
            font-size: 10px;
            padding: 5px 25px 5px 25px;
            margin-top: 11px;
            border-radius: 20px;
            color: white;
            background-color: $darklightgreen;
          }
        }
      }

      .learn_more {
        width: 65%;
        height: 100%;
        // background-color: peru;
        display: flex;

        .item {
          width: 150px;
          height: 270px;
          margin: 50px 10px;
          // background-color: rgb(0, 255, 64);
          // border: 1px solid black;
          display: flex;
          flex-direction: column;
          // justify-content: center;
          align-items: center;

          .item_square {
            width: 90%;
            height: 130px;
            // background-color: red;
            // border: 1px solid black;

            img {
              width: 100%;
              height: 100%;
            }
          }

          h5 {
            margin: 10px;
            color: $headergray;
          }

          .button {
            padding: 3px 8px;
            border: 2px solid $headergray;
            border-radius: 20px;
            font-size: 10px;
          }
        }
      }
    }
  }
}

// / SECTION COMMERCIAL
</style>
