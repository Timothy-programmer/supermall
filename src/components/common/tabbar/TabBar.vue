<template>
  <div id="tab-bar">
    <slot></slot>
  </div>
</template>

<script>
  export default {
    name:'tabBar'
  }
</script>

<style scoped>
  #tab-bar{
    background-color: rgba(218, 224, 228, 0.863);
    box-shadow: 0 -3px 1px #ccc;
    display: flex;
    position: fixed;
    left: 0px;
    right: 0px;
    bottom: 0px;
    
  }
  
</style>