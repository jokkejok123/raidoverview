<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <RaidBots msg="Simbot data here:" />
  </div>
</template>

<script>
import RaidBots from '@/components/RaidBots.vue'

export default {
  name: 'Home',
  components: {
    RaidBots
  }
}
</script>
