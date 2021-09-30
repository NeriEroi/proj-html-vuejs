<template>
  <header>
    <!-- <img src="../assets/images/driving_preview.jpg" alt=""> -->

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

header {
  ul {
    li .new::after {
      width: 10px;
      height: 10px;
      background-color: lime;
      content: "new";
    }
  }
}

</style>