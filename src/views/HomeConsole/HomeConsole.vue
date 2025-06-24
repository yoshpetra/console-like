<template>
  <main contenteditable>
    {{ renderData }}
  </main>
</template>

<script setup>
import { onMounted, ref, computed } from 'vue'

const rawData = ref('')
const renderData = computed(() => {
  return rawData
})

onMounted(() => {
  rawData.value = 'initializing...\n'
})
</script>

<style lang="scss" src="./HomeConsole.scss"></style>
