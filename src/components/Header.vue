<template>
  <header>
    <!-- <img src="../assets/images/driving_preview.jpg" alt=""> -->

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

    <ul>
      <li v-for="(headerLink, index) in headerLinks" :key="index">
        <a :class="(headerLink.status) ? 'new' : null" href="#">
          {{ headerLink.text }}
        </a>
      </li>

      <li>
          BOOK NOW
      </li>
    </ul>
    
  </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
      return {
        headerLinks: [
          {
            text: "home",
            status: false
          },
          {
            text: "about",
            status: false
          },
          {
            text: "prices",
            status: false
          },
          {
            text: "courses",
            status: true
          },
          {
            text: "locations",
            status: false
          },
          {
            text: "blog",
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

  .sub_header {
    height: 35px;
    background-color: $headergray;
    display: flex;

    section {
      height: 100%;
      width: calc(100% / 2);
      // background-color: magenta;
      // border: 1px solid black;
      display: flex;
      justify-content: center;
      align-items: center;

      h5 {
        color: $gray;
        font-size: 10px;

        i {
          margin-right: 10px;
        }
      }
    }
  }

  ul {
    li a {
      color: lime;
      text-decoration: none;

      .new::after {
      width: 10px;
      height: 10px;
      background-color: lime;
      content: "new";
      }
    }
  }
}

</style>