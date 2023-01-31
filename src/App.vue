<template>
  <div
    class="bg-red-300 h-[200px] bg-banner bg-auto flex justify-start items-end text-white">
    <span class="p-1 text-xs font-bold">{{ date }}</span>
  </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue'
const date = ref(0)
setInterval(() => {
  date.value = date.value++
}, 1000)
</script>
