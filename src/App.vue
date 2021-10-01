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

        <div class="commercial_bottom">
          
        </div>

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
          height: 35px;
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

// SECTION COURSES
section.commercial {
  width: 100%;
  height: 500px;
  background-color: lawngreen;

  .commercial_top {
    width: 100%;
    height: 100%;

    .commercial_top_wrap {
      width: 60%;
      height: 165px;
      margin: auto;
      background-color: mediumblue;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
  }
}

// / SECTION COURSES
</style>
