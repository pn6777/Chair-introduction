<script>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>

    <div class="header">
        <a href=""><img src="../../font.png" alt=""></a>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
    </div>

</template>

<style scpoed lang="scss">
body{
    background-color: #FFFBE2;
}

.header{
    height: 10vh;
    padding: 0 13vw;
    position: fixed;
    top: 0%;
    background-color: pink;
    z-index: 1;
}
</style>