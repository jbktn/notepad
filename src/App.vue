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
    background-color: rgb(17 24 39);
    color: aliceblue;
  }
  .home{
    font-size: 2rem;
    font-weight: 600;

  }
  .navlinks{
    font-size: 1.25rem;
    font-weight: 300;
    position: absolute;
    top: 8px;
    right: 3rem;
    display: flex;
    justify-content: space-between;
  }
  .navbutton{

  }
</style>
