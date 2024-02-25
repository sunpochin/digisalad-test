<script setup>
import AOS from 'aos'
import 'aos/dist/aos.css'
import { onMounted } from 'vue'
import { RouterView } from 'vue-router'

onMounted(() => {
  AOS.init()
})
</script>

<template>
  <RouterView />
</template>

<style scoped></style>
