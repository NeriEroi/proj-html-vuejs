<template>
  <header>

    <!-- sub header -->
      <div class="sub_header">

        <section>
          <h5>
            We have a 95% Succssful Pass Rate!
          </h5>
        </section>

        <section>
          <h5>
            <i class="fas fa-phone"></i>
            Give us a call to book your tuition! 1-800-555-555
          </h5>
        </section>

      </div>
    <!-- / sub header -->

    <!-- nav  -->
      <div id="nav_line">

        <div class="opacity">

          <nav>

            <div class="logo_cont">

              <img src="../assets/images/avada-drivers-logo-1x.png" alt="avada drivers logo">

            </div>

            <ul>
              <li v-for="(headerLink, index) in headerLinks" :key="index">
                <a :class="(headerLink.status) ? 'new' : null" href="#">
                  {{ headerLink.text }}
                </a>
              </li>

              <li class="book_now">
                  BOOK NOW
              </li>
            </ul>

          </nav>

        </div>

      </div>      
    <!-- / nav  -->

    <div class="text_cont">

      <h1>
        Drive with Avada
      </h1>

      <p>
        We offer the finest driving tuition money can buy
      </p>

    </div>

    <div class="details_cont">

      <div class="demos_cont">

        <i class="fab fa-accusoft"></i>

        <p>
          Demos
        </p>

      </div>

      <div class="sale_cont">

        <div class="price">

          <div class="dollar_symbol">

            <i class="fas fa-dollar-sign"></i>

            <span>39</span>

          </div>

        </div>

        <p>
          On Sale
        </p>

      </div>

    </div>

  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      headerLinks: [
        {
          text: "HOME",
          status: false,
        },
        {
          text: "ABOUT",
          status: false
        },
        {
          text: "PRICES",
          status: false
        },
        {
          text: "COURSES",
          status: true
        },
        {
          text: "LOCATIONS",
          status: false
        },
        {
          text: "BLOG",
          status: false
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

header {
  width: 100%;
  position: relative;
  background-color: $headergray;

  .sub_header {
    width: 60%;
    height: 35px;
    margin: auto;
    display: flex;
    justify-content: space-between;
    align-items: center;

    section {
      
      h5 {
        color: $gray;
        font-size: 10px;

        i {
          margin-right: 10px;
        }
      }
    }
  }

  #nav_line {
    width: 100%;
    height: 600px;
    background-image: url("../assets/images/homepage-hero-background.jpg");
    background-repeat: no-repeat;
    background-size: cover;

    .opacity {
      width: 100%;
      background-color: $headergray;
      opacity: 0.7;

      nav {
        width: 62%;
        height: 130px;
        margin: auto;
        display: flex;
        justify-content: space-between;

        .logo_cont {
          padding: 10px;
          display: flex;
          align-items: center;
        }

        ul {
          display: flex;
          align-items: center;

          li {
            height: 20px;
            list-style-type: none;
            padding: 15px;
            font-size: 12px;
            color: white;
            cursor: pointer;

            :hover {
              color: $lightgreen;
              border-bottom: 2px solid $lightgreen;
              padding-bottom: 10px;
            }

            a {
              color: white;
              text-decoration: none;
              font-size: 12px;
            }

            .new::after {
              padding: 1px 8px;
              background-color: $lightgreen;
              border-radius: 10px;
              content: "new";
              color: white;
            }
          }

          .book_now {
            height: 30px;
            padding: 5px 15px;
            margin-bottom: -20px;
            border-radius: 10px;
            background-color: $lightgreen;
            color: white;
          }
        }
      }
    }
  }

  .text_cont {
    position: absolute;
    left: 20%;
    bottom: 30%;
    color: white;
    font-size: 20px;
  }

  .details_cont {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    position: absolute;
    right: 0;
    top: 22%;
    z-index: 999;

    .demos_cont {
      width: 70px;
      height: 70px;
      margin-top: 10px;
      margin-right: 10px;
      background-color: white;
      border-radius: 10px;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      align-items: center;
      box-shadow: 0 0 3px $darklightgreen, 0 0 5px $lightgreen;

      i {
        margin-top: 20px;
        font-size: 20px;
        font-weight: 900;
        color: rgba(20, 20, 240, 0.979);
      }

      p {
        font-size: 13px;
        font-weight: 900;
      }
    }

    .sale_cont {
      width: 70px;
      height: 70px;
      padding-top: 10px;
      margin-top: 10px;
      margin-right: 10px;
      background-color: white;
      border-radius: 10px;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      box-shadow: 0 0 3px $darklightgreen, 0 0 5px $lightgreen;

      .price {
        display: flex;
        font-weight: 900;
        color: green;

        .dollar_symbol {
          font-size: 20px;
          margin-bottom: -11px;

          i {
            font-size: 13px;
            vertical-align: text-top;
          }

          span {
            font-size: 30px;
            font-weight: 900;
          }
        }
      }

      p {
        font-size: 13px;
        font-weight: 900;
      }
    }
  }
}

</style>