<script setup>
import AboutComp from '@/components/AboutComp.vue'
</script>

<template>
  <div class="full-width">
    <section>Video</section>
    <AboutComp />
    <section>Awards</section>
    <section>Ingradients</section>
    <section>Founder</section>
    <section>Brand Experience</section>
    <section>Highlighted Showcase</section>
  </div>
</template>

<style scoped>
.full-width {
  width: 100%;
  padding: 0;
  margin: 0;
}
html,
body {
  width: 100%;
  margin: 0;
  padding: 0;
  overflow-x: hidden; /* 防止水平滾動 */
}
</style>
