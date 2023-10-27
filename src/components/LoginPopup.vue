<script default>
  props: ['popup']
</script>

<template>
  <div class="login-popup">
    <h2>Login</h2>
    <input type="text">
    <input type="password">
  </div>
</template>

<style>
  .login-popup {
    background-color: #AAA9EF;
    position: absolute;
    z-index: 100;
    top: 50%;
    left: 50%;
    margin: -7.5rem 0 0 -10rem;
    align-items: center;
    width: 15rem;
    height: 20rem;
  }
</style>