<template>
  <header>
    <!-- <img src="../assets/images/driving_preview.jpg" alt=""> -->

    <ul v-for="(headerLink, index) in headerLinks" :key="index">
      <li>
        {{ headerLink.text }}
      </li>
    </ul>

    <div class="button_cont">
      <div class="button">
        BOOK KNOW
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
            text: "home"
          },
          {
            text: "about"
          },
          {
            text: "prices"
          },
          {
            text: "courses"
          },
          {
            text: "locations"
          },
          {
            text: "blog"
          },
        ]
      }
    }
}
</script>

<style scoped lang="scss">
@import "../style/generals";
@import "../style/vars";

</style>