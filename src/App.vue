<script setup>

</script>

<template>
  <header>
    <div class="home">
      <router-link style="text-decoration: none; color: inherit;" to='/'>
        Notepad
      </router-link>
    </div>
    <div class="navlinks">
      <div class="navbutton">
        <router-link style="text-decoration: none; color: inherit;" to='/Login'>login</router-link>
      </div>
      <div class="navbutton">
        <router-link style="text-decoration: none; color: inherit;" to='/Register'>register</router-link>
      </div>
    </div>
  </header>
  <router-view/>
</template>

<style scoped>

  header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 10%;
    background-color: rgb(5 5 5);
    overflow: hidden;
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 9999;
    font-size: larger;
    color: aliceblue;
  }
  .home{
    font-size: 2rem;
    font-weight: 600;
  }
  .navlinks{
    font-size: 1.25rem;
    font-weight: 300;

  }
  .navbutton{

  }
</style>
