<template>
    <button @click="sendMsg()">-</button>
</template>

<script>
import { EventBus } from '../util/eventBus.js'
export default {
  methods: {
    sendMsg () {
      EventBus.$emit('aMsg', '来自A页面的消息')
    }
  }
}
</script>
