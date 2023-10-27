<script default>
  props: ['popup']
</script>

<template>
  <div class="login-popup">
    <h2>Login</h2>
    <input class="box" type="text" PLACEHOLDER="login">
    <input class="box" type="password" placeholder="password">
    <button class="register-button">Login</button>
  </div>
</template>

<style>
  input::placeholder {
    text-align: center;
  }
  .login-popup {
    font-size: 150%;
    background-color: #AAA9EF;
    border-radius: 1rem;
    text-align: center;
    position: absolute;
    z-index: 100;
    top: 50%;
    left: 50%;
    margin: -7.5rem 0 0 -10rem;
    align-items: center;
    width: 15rem;
    height: 20rem;
  }
  .register-button {
    background-color: black;
    border-radius: 0.75rem;
    border: none;
    color: white;
    padding: 0.2rem 2rem;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 90%;
    margin-top: 1.5rem;
    cursor: pointer;
  }
  .box {
    font-size: 65%;
    margin: 2px;
  }
</style>