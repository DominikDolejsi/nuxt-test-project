<script lang="ts" setup>
definePageMeta({ middleware: ['auth'] })
const count = ref(1)
const double = computed(() => count.value * 2)
const { data, refresh, pending } = await useAsyncData('/api/hello', () => $fetch('/api/hello'))
</script>

<template>
  
</template>

<style scoped>
  
</style>
