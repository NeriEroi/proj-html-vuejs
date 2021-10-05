<template>
  <!-- STATS AND INSTRUCTORS  -->
  <section class="stats_instructors">

    <div class="down_arrow">

      <img src="../assets/images/driving-triangle.svg" alt="driving triangle">

    </div>

    <div class="rate_cont">

      <div class="rate_wrap">

        <div class="item">

          <div class="circle_cont">

            <div class="circle_left">

              <span>95%</span>

            </div>
            
          </div>

          <div class="description_cont">

            <span>PASS RATE</span>

          </div>

        </div>

        <div class="item">

          <div class="circle_cont">

            <div class="circle">

              <span>100%</span>

            </div>

          </div>

          <div class="description_cont">

            <span>REFERRAL RATE</span>

          </div>

        </div>

        <div class="item">

          <div class="circle_cont">

            <div class="circle_right">

              <span>0%</span>

            </div>

          </div>

          <div class="description_cont">

            <span>ACCIDENT RATE</span>

          </div>

        </div>

      </div>

    </div>

    <div class="instructors_cont">

      <div class="instructors_wrap">

        <div class="text_wrap">

          <div>

            <h1>
            Your Instructors
            </h1>
            <p>
              Lorem ipsum dolor, sit amet consectetur adipisicing elit. Doloremque voluptatem
              similique quos minima voluptates maxime velit 
            </p>

          </div>

        </div>

        <div class="button_wrap">

          <div class="button">
            <p>
              MORE ABOUT US
            </p>
          </div>

        </div>
        
      </div>

    </div>

    <div class="photos_instructors_cont">

      <div class="photos_instructors_wrap">

        <div class="item">

          <div class="photo_cont">

            <img src="../assets/images/instructor-mikehart-200x127.jpg" alt="instructor mike hart">
            
          </div>

          <div class="description_cont">

            <h3>Mike Hart</h3>

            <div class="logos_cont">
              <div class="logos">
                <i class="fab fa-facebook-f"></i>
                <i class="fab fa-twitter"></i>
                <i class="fab fa-instagram"></i>
              </div>
            </div>

            <p>
              Lorem ipsum dolor sit amet, 
              consectetur adipisicing elit. 
            </p>

          </div>

        </div>

        <div class="item">

          <div class="photo_cont">

            <img src="../assets/images/instructor-johnsmith-200x127.jpg" alt="instructor john smith">
            
          </div>

          <div class="description_cont">

            <h3>John Smith</h3>

            <div class="logos_cont">
              <div class="logos">
                <i class="fab fa-facebook-f"></i>
                <i class="fab fa-twitter"></i>
                <i class="fab fa-instagram"></i>
              </div>
            </div>

            <p>
              Lorem ipsum dolor sit amet, 
              consectetur adipisicing elit. 
            </p>

          </div>

        </div>

        <div class="item">

          <div class="photo_cont">

            <img src="../assets/images/instructor-angelahart-200x127.jpg" alt="instructor angela hart">
            
          </div>

          <div class="description_cont">

            <h3>Angela Hart</h3>

            <div class="logos_cont">
              <div class="logos">
                <i class="fab fa-facebook-f"></i>
                <i class="fab fa-twitter"></i>
                <i class="fab fa-instagram"></i>
              </div>
            </div>

            <p>
              Lorem ipsum dolor sit amet, 
              consectetur adipisicing elit. 
            </p>

          </div>

        </div>

      </div>

    </div>

  </section>
  <!-- / STATS AND INSTRUCTORS  -->
</template>

<script>
export default {
  name: 'StatsAndInstructors',
}
</script>

<style scoped lang="scss">
@import "../style/generals";
@import "../style/vars";
@import '~@fortawesome/fontawesome-free/css/all.min.css';

// STATS AND INSTRUCTORS
.stats_instructors .down_arrow img {
  width: 100%;
  height: 100px;
}

.stats_instructors .rate_cont {
  width: 100%;
  height: 355px;
  // background-color: chartreuse;

  .rate_wrap {
    width: 60%;
    height: 100%;
    // background-color: chocolate;
    margin: auto;
    margin-top: -100px;
    display: flex;

    .item {
      width: 295px;
      height: 300px;
      // border: 1px solid black;
      border-radius: 10px;
      background: linear-gradient(to top, white 99%, #79b27b 1%);
      box-shadow: 0px 10px #e7e4e4;

      .circle_cont {
        width: 100%;
        height: 50%;
        // background-color: darkorchid;
        display: flex;
        justify-content: center;
        align-items: center;

        .circle {
          width: 130px;
          height: 130px;
          margin-top: 50px;
          border-radius: 50%;
          border-top: 0.4em solid $darklightgreen;
          border-right: 0.4em solid $darklightgreen;
          border-bottom: 0.4em solid $darklightgreen;
          border-left: 0.4em solid $darklightgreen;
          display: flex;
          justify-content: center;
          align-items: center;

          span {
            font-size: 25px;
            color: $gray;
          }
        }

        .circle_left {
          width: 130px;
          height: 130px;
          margin-top: 50px;
          border-radius: 50%;
          border-top: 0.4em solid rgba(0, 0, 0, 0.2);
          border-right: 0.4em solid $darklightgreen;
          border-bottom: 0.4em solid $darklightgreen;
          border-left: 0.4em solid $darklightgreen;
          display: flex;
          justify-content: center;
          align-items: center;

          span {
            font-size: 25px;
            color: $gray;
          }
        }

        .circle_right {
          width: 130px;
          height: 130px;
          margin-top: 50px;
          border-radius: 50%;
          border-top: 0.4em solid $darklightgreen;
          border-right: 0.4em solid rgba(0, 0, 0, 0.2);
          border-bottom: 0.4em solid rgba(0, 0, 0, 0.2);
          border-left: 0.4em solid rgba(0, 0, 0, 0.2);
          display: flex;
          justify-content: center;
          align-items: center;

          span {
            font-size: 25px;
            color: $gray;
          }
        }
      }

      .description_cont {
        display: flex;
        justify-content: center;
        align-items: center;

        span {
          margin-top: 50px;
          color: $gray;
        }
      }
    }

    .item:nth-of-type(2) {
      margin: 0 auto;
    }
  }
}

.stats_instructors .instructors_cont {
  width: 100%;
  height: 150px;
  // margin-bottom: 50px;
  // background-color: yellowgreen;

  .instructors_wrap {
    width: 60%;
    height: 100%;
    // background-color: chocolate;
    margin: auto;
    display: flex;

    .text_wrap {
      width: 60%;
      // background-color: tomato;
      display: flex;
      align-items: center;
    }

    .button_wrap {
      width: 40%;
      // background-color: yellow;
      display: flex;
      justify-content: flex-end;
      align-items: center;

      .button {
        padding: 5px 80px;
        background-color: $darklightgreen;
        border-radius: 20px;
        cursor: pointer;
        
        p {
          color: white;
          font-size: 13px;
        }
      }
    }
  }
}

.stats_instructors .photos_instructors_cont {
  width: 100%;
  height: 355px;
  // background-color: chartreuse;

  .photos_instructors_wrap {
    width: 60%;
    height: 100%;
    // background-color: chocolate;
    position: relative;
    bottom: -60px;
    margin: auto;
    display: flex;

    .item {
      width: 290px;
      height: 340px;
      // border: 1px solid black;
      border-radius: 10px;
      background: linear-gradient(to top, white 99%, #79b27b 1%);
      box-shadow: 5px 5px 5px 5px #a79e9e75;
      display: flex;
      flex-direction: column;
      align-items: center;

      .photo_cont {
        width: 200px;
        height: 127px;
        margin-top: 25px;
        // background-color: tomato;

      }

      .description_cont {
        display: flex;
        flex-direction: column;
        align-items: center;
      }

      h3 {
        margin-top: 25px;
        color: $footer;
      }

      .logos_cont .logos i {
        margin-top: 10px;
        color: $gray;
      }

      .logos_cont .logos i:nth-of-type(2) {
        margin: 0 10px;
        color: $gray;
      }

      p {
        margin-top: 10px;
        text-align: center;
        font-size: 13px;
        color: $gray;
      }
    }

    .item:nth-of-type(2) {
      margin: 0 auto;
      height: 350px;
    }
  }
}
// / STATS AND INSTRUCTORS
</style>