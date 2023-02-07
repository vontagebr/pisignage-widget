<template>
  <div class="text-white bg-blue-200 relative">
    <img src="/img/banner.png" class="bject-cover w-full" />
    <div class="absolute top-0 w-full h-full flex items-center justify-center">
      <span class="text-xs font-bold z-10">{{ date }}</span>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { ref, unref } from 'vue'
const date = ref(0)
setInterval(() => {
  date.value = unref(date) + 1
}, 100)
</script>
