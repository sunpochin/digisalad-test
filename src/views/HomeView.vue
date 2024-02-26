<script setup>
// import HeaderComp from '@/components/HeaderComp.vue'
import TasteComp from '@/components/TasteComp.vue'
import AboutComp from '@/components/AboutComp.vue'
import AwardsComp from '@/components/AwardsComp.vue'
import Ingradients from '@/components/IngradientsComp.vue'
</script>

<template>
  <div class="home">
    <!-- <HeaderComp /> -->
    <TasteComp />
    <AboutComp />
    <AwardsComp />
    <Ingradients />
    <section>Founder</section>
    <section>Brand Experience</section>
    <section>Highlighted Showcase</section>
  </div>
</template>

<style lang="scss" scoped>
.home {
  width: 100%;
  max-width: 100%;
  margin: auto;
}
</style>
