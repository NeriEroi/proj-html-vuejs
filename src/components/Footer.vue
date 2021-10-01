<template>
  <footer>
    
    <section class="footer_top">

      <div class="box">

        <section>

        </section>

        <section>

        </section>

        <section>

        </section>

        <section>

        </section>

      </div>

    </section>

    <section class="footer_bottom">

      <div class="box">

        <section>

        </section>

        <section>

        </section>
        
      </div>
      
    </section>

  </footer>
</template>

<script>
export default {
    name: 'Footer',
}
</script>

<style scoped lang="scss">

.footer_top {
  width: 100%;
  height: 380px;
  background-color: rgb(55, 0, 255);

  .box section {
    width: calc(100% / 4);
    height: 100%;
    background-color: rgb(0, 255, 21);
    border: 1px solid black;
  }
}
.footer_bottom {
  width: 100%;
  height: 120px;
  background-color: rgb(55, 0, 255);

  .box section {
    width: calc(100% / 2);
    height: 100%;
    background-color: rgb(255, 0, 0);
    border: 1px solid black;
  }
}
.box {
  width: 75%;
  height: 100%;
  margin: auto;
  background-color: darkolivegreen;
  display: flex;
}

</style>