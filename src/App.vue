<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/login">Login</router-link>
    </div>
    <router-view />
  </div>
</template>
<script>
import '@/assets/scss/stylesheet.scss'

export default {
  data() {
    return {
      test: true
    }
  }
}
</script>
