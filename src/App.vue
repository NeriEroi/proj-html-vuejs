<template>
  <div id="app">

    <Header />

    <main>

      <Request />

      <Commercial />

      <StatsAndInstructors />

      <Testimonials />

      <LatestNews />

      <NewsLetter />

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
import LatestNews from './components/LatestNews.vue'
import NewsLetter from './components/NewsLetter.vue'
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    Header,
    Request,
    Commercial,
    StatsAndInstructors,
    Testimonials,
    LatestNews,
    NewsLetter,
    Footer,
  }
}
</script>

<style lang="scss">
@import "./style/generals";
@import "./style/vars";
</style>
