<template>
  <div id="app">

    <Header />

    <main>

      <Request />

      <Commercial />

      <StatsAndInstructors />

      <Testimonials />

      

      <!-- LATEST NEWS  -->
      <section class="latest_news">

        <div class="news_box">

          <div class="title_cont">
            <h3>
              Latest News
            </h3>
          </div>

          <div class="items_cont">

            <div class="item">

              <div class="image_cont">
                <img src="./assets/images/blog-choosecar-320x202.jpg" alt="choosecar">
              </div>

              <div class="text">
                <h3>
                  What car to start with?
                </h3>
                <p>
                  February 7th, 2019 | 0 Comments
                </p>
                <p>
                  Lorem ipsum dolor sit amet consectetur adipisicing
                </p>
              </div>

            </div>

            <div class="item">

              <div class="image_cont">
                <img src="./assets/images/blogpost-10and2-320x202.jpg" alt="10and2">
              </div>

              <div class="text">
                <h3>
                  Avada Driving School Expanding
                </h3>
                <p>
                  February 7th, 2019 | 0 Comments
                </p>
                <p>
                  Lorem ipsum dolor sit amet consectetur adipisicing
                </p>
              </div>

            </div>

          </div>

          <div class="button">
            <p>
              MORE FROM THE BLOG
            </p>
          </div>

        </div>

        <div class="triangle">
          <img src="./assets/images/driving-triangle.svg" alt="driving triangle">
        </div>

      </section>
      <!-- / LATEST NEWS  -->

      <!-- NEWSLETTER  -->
      <section class="newsletter">

        <div class="newsletter_wrap">

          <h1>
            Sign up to our Newsletter
          </h1>

          <input type="text">

          <div class="button">
            SUBSCRIBE
          </div>

          <p>
            (We do not share your data with anybody, and only use it for its intended purpose)
          </p>

        </div>

      </section>
      <!-- / NEWSLETTER  -->
    </main>

    <Footer />
    
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Request from './components/Request.vue'
import Commercial from './components/Commercial.vue'
import StatsAndInstructors from './components/StatsAndInstructors.vue'
import Testimonials from './components/Testimonials.vue'
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    Header,
    Request,
    Commercial,
    StatsAndInstructors,
    Testimonials,
    Footer,
  }
}
</script>

<style lang="scss">
@import "./style/generals";
@import "./style/vars";





// LATEST NEWS
.latest_news {
  width: 100%;
  height: 600px;
  background-image: url("./assets/images/latestnews-background.jpg");
  background-size: cover;

  .news_box {
    width: 60%;
    height: 85%;
    margin: 0 auto;
    background: linear-gradient(to top, #E4EAED 99%, $gumbo 1%);
    position: relative;
    top: -35px;
    border-top-left-radius: 10px;
    border-top-right-radius: 10px;

    .title_cont {
      text-align: center;

      h3 {
        padding-top: 50px;
        padding-bottom: 25px;
        font-size: 25px;
      }
    }

    .items_cont {
      height: 65%;
      // background-color: yellowgreen;
      display: flex;

      .item {
        width: 50%;
        height: 100%;
        // background-color: yellow;
        // border: 3px solid black;

        .image_cont {
          width: 80%;
          height: 60%;
          margin: auto;
          // background-color: teal;

          img {
            width: 100%;
            height: 100%;
          }
        }

        .text {
          text-align: center;

          h3 {
            padding-top: 10px;
            color: $lightgreen;
          }

          p {
            padding: 3px;
            color: $gray;
          }
        }
      }
    }

    .button {
      display: flex;
      justify-content: center;

      p {
        width: 210px;
        padding: 5px 10px;
        margin-top: 20px;
        font-size: 15px;
        background-color: $lightgreen;
        border-radius: 20px;
        text-align: center;
        color: white;
        cursor: pointer;
      }
    }
  }

  .triangle {
    width: 60%;
    height: 85px;
    margin: 0 auto;
    position: relative;
    top: -35px;

    img {
      width: 100%;
      height: 100%;
    }
  }
}
// / LATEST NEWS

// NEWSLETTER
.newsletter {
  width: 100%;
  height: 350px;
  background-image: url("./assets/images/newsletter_background.jpg");
  background-size: cover;

  .newsletter_wrap {
    width: 60%;
    height: 100%;
    // background-color: tomato;
    margin: auto;
    display: flex;
    flex-direction: column;
    align-items: center;

    h1 {
      margin-top: 35px;
    }

    input {
      width: 550px;
      padding: 20px;
      margin-top: 35px;
    }

    .button {
      width: 550px;
      padding: 3px;
      margin: 20px 0;
      background-color: $lightgreen;
      text-align: center;
      border-radius: 20px;
      color: white;
      cursor: pointer;
    }

    p {
      font-size: 13px;
      color: $gray;
    }
  }
}

// / NEWSLETTER
</style>
