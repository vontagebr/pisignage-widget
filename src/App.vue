<template>
  <div
    class="bg-red-300 h-[200px] bg-banner bg-auto flex justify-center items-end text-white">
    <span class="p-1 text-xs">{{ date }}</span>
  </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue'
const date = ref(new Date().toISOString())
setInterval(() => {
  date.value = new Date().toISOString()
}, 100)
</script>
