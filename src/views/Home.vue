<script>
  import LoginPopup from '@/components/LoginPopup.vue'
  export default {
    name: 'Home',
    components: {
      LoginPopup
    }
  }
</script>

<template>
  <div class="content">
    <h1 class="content-slogan">Single <span class="content-slogan-gradient">Notepad</span> for all your needs</h1>
  </div>
  <div class="textbox">
    <textarea placeholder="Start typing..." cols="40" rows="5" class="text"></textarea>
  </div>
</template>

<style scoped>
  .textbox {
    margin: auto;
    color: black;
    width: 80%;
    height: 50rem;
  }
  .text {
    width: 100%;
    height: 100%;
  }
</style>