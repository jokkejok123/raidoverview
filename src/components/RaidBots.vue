<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>{{ raidbots.simbot.input }}</p>
  </div>
</template>

<script>
import simdata from '@/data.json'

export default {
  name: 'RaidBots',
  props: {
    msg: String
  },
  data() {
    return {
      raidbots: simdata
    }
  }
}
</script>
