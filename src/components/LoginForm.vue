<template>
  <div>
    <form action="">
      <input
        type="email"
        name="email"
        id="email"
        placeholder="email"
        v-model="input.email"
      />
      <input
        type="password"
        name="pass"
        id="password"
        placeholder="password"
        v-model="input.password"
      />
      <button type="button" @click="login()">Login</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      input: {
        email: '',
        password: ''
      }
    }
  },
  methods: {
    login() {
      if (this.input.username != '' && this.input.password != '') {
        if (
          this.input.username == this.$parent.mockAccount.username &&
          this.input.password == this.$parent.mockAccount.password
        ) {
          this.$emit('authenticated', true)
          this.$router.replace({ name: 'secure' })
        } else {
          console.log('The username and / or password is incorrect')
        }
      } else {
        console.log('A username and password must be present')
      }
    }
  }
}
</script>

<style></style>
