<script setup>

</script>

<template>
  <div class="navbar">
    <header class="navbar-header">
      <div class="navbar-homebutton">
        <router-link style="text-decoration: none; color: inherit;" to='/'>
          @ Notepad
        </router-link>
      </div>
      <div class="navbar-navlinks">
        <button @click="toggleLoginPopup" class="navbar-navbutton">
          Login
<!--          <router-link to='/Login'>login</router-link>-->
        </button>
        <div class="navbar-navbutton">
          <router-link to='/Register'>register</router-link>
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
