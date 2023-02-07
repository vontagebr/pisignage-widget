<template>
  <div class="h-screen text-white relative flex justify-center items-center">
    <img src="/img/banner.png" class="absolute h-full -z-10" />
    <span class="p-1 text-xs font-bold z-10">{{ date }}</span>
  </div>
</template>

<script lang="ts" setup>
import { ref, unref } from 'vue'
const date = ref(0)
setInterval(() => {
  date.value = unref(date) + 1
}, 100)
</script>
