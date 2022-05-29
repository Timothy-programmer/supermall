<template>
    <div class="tab-bar-item" @click="itemclick">
      <slot v-if="!isActive"  name="item-icon"></slot>
      <slot v-else name="item-icon-active"></slot>
      <slot name="item-text"></slot>
    </div>
</template>

<script>
  export default {
    name:'TabBarItem',
    props:{
          path:String
        },
    
    data(){
      return{    
      }
    },
    computed:{
      isActive(){
        return this.$route.path === this.path;
        
      }
    },
    methods: {
      itemclick(){
        this.$router.replace(this.path)
        console.log("itemclick");
      }
    },
  }
 
</script>

<style>
  .tab-bar-item{
    height: 49px;
    flex:1;
    text-align: center;
    font-size:14px;
  }
  .tab-bar-item img{
    width: 24px;
    height: 24px;
    
  }
</style>