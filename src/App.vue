<script setup>
import { RouterView } from 'vue-router';
</script>

<template>
  <!-- <div class="header">
      <Header />
  </div> -->

  <div class="content">
    <RouterView />
  </div>
</template>

<style scoped lang="scss">
.header {
  height: 10vh;
}

.content {
  width: 100vw;
}
</style>
