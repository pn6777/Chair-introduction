<script>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>

    <div class="linkedin">
        <RouterLink to="/"><img src="../../font.png" alt=""></RouterLink>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
    </div>

</template>

<style scpoed lang="scss">
body{
    background-color: #FFFBE2;
}

.linkedin{
    height: 7vh;
    padding: 0 13vw;
    margin: 0 30vw;
    border-radius: 30px;
    position: fixed;
    top: 3%;
    background-color: rgb(184, 226, 159);
    z-index: 1;
}
</style>