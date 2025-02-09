<script setup>
import AlertComponent from './components/AlertComponent.vue';


</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <AlertComponent msg="Hello Rayhan" type="Success"/>
      <br>
      <alert-component msg="Hey" type="error"/>
   
    </div>
  </header>

  <main>
    
   
  </main>
</template>

<style scoped>

</style>