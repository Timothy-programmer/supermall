<template>
  <div id="home">
    <nav-bar class="home-nav">
      <template v-slot:center>MoGuGai</template>
    </nav-bar>
    首页

  </div>
</template>

<script>
import NavBar from "@/components/common/navbar/NavBar";
  export default {
    components:{
      NavBar
    }
  }
</script>

<style scoped>
  .home-nav{
    background-color:var(--color-tint);
    color: var(--color-text);
  }
</style>