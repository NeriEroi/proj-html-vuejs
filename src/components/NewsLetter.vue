<template>
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
</template>

<script>
export default {
  name: 'NewsLetter',
}
</script>

<style scoped lang="scss">
@import "../style/generals";
@import "../style/vars";
@import '~@fortawesome/fontawesome-free/css/all.min.css';

// NEWSLETTER
.newsletter {
  width: 100%;
  height: 350px;
  background-image: url("../assets/images/newsletter_background.jpg");
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