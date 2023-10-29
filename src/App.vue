<style>
  .navbar-navbutton-l{
    color: var(--text);
    border: none;
    border-top: 2px solid var(--Primary);
    border-bottom: 2px solid var(--Primary);
    border-left: 2px solid var(--Primary);
    border-bottom-left-radius: 1rem;
    border-top-left-radius: 1rem;
    padding: 0.1rem 1rem;
    background-color: var(--Secondary);
    font-size: 1.1rem;
    font-weight: bolder;
  }
  .navbar-navbutton-r{
    color: var(--text);
    border: 2px solid var(--Primary);
    border-bottom-right-radius: 1rem;
    border-top-right-radius: 1rem;
    padding: 0.1rem 1rem;
    background-color: var(--Secondary);
    font-size: 1.1rem;
    font-weight: bolder;
    text-decoration: none;
  }
</style>

<template>
  <div class="navbar">
    <header class="navbar-header">
      <div class="navbar-homebutton">
        <router-link style="text-decoration: none; color: inherit;" to='/'>
          @ Notepad
        </router-link>
      </div>
      <div class="navbar-navlinks">
        <button @click="toggleLoginPopup" class="navbar-navbutton-l">
          Login
<!--          <router-link to='/Login'>login</router-link>-->
        </button>
        <div class="navbar-navbutton-r">
          <router-link to='/Register'>Register</router-link>
        </div>
      </div>
    </header>
  </div>
  <router-view/>

  <LoginPopup
    v-if="showLoginPopup"
  />

</template>

<script>
import LoginPopup from '@/components/LoginPopup.vue'

export default {
  components: {
    LoginPopup
  },
  data () {
    return {
      showLoginPopup: false
    }
  },
  methods: {
    toggleLoginPopup () {
      this.showLoginPopup = !this.showLoginPopup
    }
  }
}
</script>
