<script setup>
import { defineComponent } from 'vue'

defineComponent({
  name: 'DocumentPreview'
})

defineProps({
  url: {
    type: String,
    default: ''
  },
  height: {
    type: [String, Number],
    default: '100%'
  }
})
</script>

<template>
  <div :style="{ height: `${height}` }">
    <iframe
      :src="`https://docs.google.com/gview?url=${url}&embedded=true`"
      width="100%"
      height="100%"
      style="border: none"
    ></iframe>
  </div>
</template>
