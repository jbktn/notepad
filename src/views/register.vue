<script setup>

</script>

<template>
  <div class="register-forms">
    <!--    <div class="login-popup-container">-->
    <h2>Register</h2>
    <div class="register-form">
      <div class="register-form-username">
        <input placeholder="Username" type="text" class="register-input">
      </div>
      <div class="register-form-email">
        <input placeholder="Email" type="email" class="register-input">
      </div>
      <div class="register-form-password">
        <input placeholder="Password" type="password" class="register-input">
      </div>
      <div class="register-form-password">
        <input placeholder="Confirm Password" type="password" class="register-input">
      </div>
      <div class="register-form-submit">
        <button class="register-form-button">Submit</button>
      </div>
    </div>
    <!--    </div>-->
  </div>
</template>

<style>
  .register-forms{
    position: absolute;
    z-index: 100;
    top: 50%;
    left: 50%;
    margin: -25rem 0 0 -7.5rem;
    align-items: center;
    width: 15rem;
    height: 30rem;
    border-radius: 10px;
    display: flex;
    align-content: center;
    flex-direction: column;
    justify-content: center;
  }
  .register-form {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }

  .register-form-username , .register-form-email {
    width: 100%;
    height: 3rem;
    padding: 1rem;
    border-radius: 10px;
    margin: 0.5rem 0;
    font-size: 0.9rem;
  }
  .register-form-password {
    width: 100%;
    height: 3rem;
    padding: 1rem;
    border-radius: 10px;
    margin: 0.5rem 0;
    font-size: 0.9rem;
  }
  .register-input {
    width: 100%;
    height: 3rem;
    padding: 1rem;
    border-radius: 10px;
    margin: 0.5rem 0;
    font-size: 0.9rem;
  }
  .register-form-submit {
    text-align: center;
    margin-top: 2rem;

  }
  .register-form-button {
    background-color: #b7b6f1;
    font-size: 1.5rem;
    width: 90%;
    height: 3rem;
    border-radius: 10px;
    margin: 0.5rem 0;
    font-weight: bolder;
    cursor: pointer;
  }
</style>

<style scoped>
  h2 {
    font-size: 4rem;
  }
</style>