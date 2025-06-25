<template>
    <div class="code">
    </div>
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

<style src="./ConsoleHistory.scss"></style>