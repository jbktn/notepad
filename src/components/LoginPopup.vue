<script default>
props: ['popup']
</script>

<template>
  <div class="login-popup">
    <h2>Login</h2>
    <div class="login-popup-form">
      <div class="login-popup-form-username">
        <input placeholder="Username" type="text" class="login-popup-input">
      </div>
      <div class="login-popup-form-password">
        <input placeholder="Password" type="password" class="login-popup-input">
      </div>
      <div class="login-popup-form-submit">
        <button class="login-popup-form-button">Submit</button>
      </div>
    </div>
  </div>
</template>

<style>
.login-popup {
  background-color:  var(--Secondary);
  position: absolute;
  z-index: 100;
  top: 50%;
  left: 50%;
  margin: -7.5rem 0 0 -7.5rem;
  align-items: center;
  width: 15rem;
  height: 20rem;
  border-radius: 10px;
  display: flex;
  align-content: center;
  flex-direction: column;
  justify-content: center;
}

.login-popup-form{
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.login-popup-input, .login-popup-form-button{
  width: 100%;
  height: 3rem;
  padding: 1rem;
  border-radius: 10px;
  margin: 0.5rem 0;
  font-size: 0.9rem;
}
</style>

<style scoped>
h2{
  font-size: 2.5rem;
  margin: 0 0 0.7rem 0;
  background: linear-gradient(90deg, #d6895c 0%, #ce713b 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.login-popup, .login-popup-input, .login-popup-form-button{
  border: solid 1px var(--Accent);
}

.login-popup-form-button{
  background-color: var(--Primary);
  font-size: 1rem;
  font-weight: bolder;
  cursor: pointer;
}

.login-popup-form-button:hover{
  background-color: #aaa9ef;
}
</style>