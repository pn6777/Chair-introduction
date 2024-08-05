<script setup>

</script>

<template>
  <main>
    <div class="topPage">
        <div class="imgDiv">
          <div class="maskDiv"></div>
        </div>
    </div>
    <!-- <div class="bottomDiv"></div> -->
  </main>
</template>

<style scoped lang="scss">
.topPage {
  width: 100vw;
  height: 70vh;
  margin-top: 20vh;

  .maskDiv{
    width: 100vw;
    height: 70vh;
    backdrop-filter: blur(5px);
  }

  .imgDiv {
    width: 100vw;
    height: 70vh;
    margin-top: 20vh;
    background-image: url("https://www.ikea.com.tw/dairyfarm/tw/pageImages/page_prev_1868_zh_tw_16866744371681051022.jpeg");
    background-repeat: no-repeat;
    background-size: 100% 100%;
  }

}
.bottomDiv{
  height: 100vh;
}
</style>
