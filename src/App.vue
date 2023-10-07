<script setup>

</script>

<template>
  <header>
    <router-link to='/'>
      Home
    </router-link>
    <router-link to='/Login'>login</router-link>
    <router-link to='/Register'>register</router-link>
  </header>
  <router-view/>
</template>

<style scoped>
  header{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    background-color: dimgray;
  }
</style>
