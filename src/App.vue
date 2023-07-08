<script setup>
import { RouterView } from 'vue-router'
import TodoHeader from './components/TodoHeader.vue';

</script>

<template>
  <TodoHeader/>
  <RouterView />
</template>

<style lang="scss" >
  nav{
    display: flex;
    justify-content: space-between;
    align-items: center;
    border: 2px solid red;
    .nav-routes{
      display: inline;
      border: 2px solid red;
    }
    .branding{
        display: flex;
        border: 2px solid red;
        justify-content: center;
        align-items: center;
        img{
            width: 80px;
            height: 80px;
        }
    }
    
  }
  
  
</style>
