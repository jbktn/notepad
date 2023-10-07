<script setup>
  import login from './components/login.vue'
  import register from './components/register.vue'
</script>

<template>
  <header>
    <div class="headtext">Notepad</div>
  </header>

  <main>

  </main>
</template>

<style scoped>
  header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 10%;
    background-color: rgb(33,51,33);
    overflow: hidden;
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 9999;
    font-size: larger;
  }
</style>
