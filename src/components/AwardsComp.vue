<template>
  <section>
    <div class="container-fluid">
      <div class="col-text">
        <TitleComp position="center" theme="primary" data-aos="fade-up">AWARDS</TitleComp>

        <p data-aos="fade-up" :data-aos-delay="100" data-aos-duration="15000">
          Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras ullamcorper bibendum
          bibendum. Duis tincidunt urna non pretium porta. Nam condimentum vitae ligula vel ornare.
          Phasellus at semper turpis. Nunc eu tellus tortor. Etiam at condimentum nisl, vitae
          sagittis orci. Donec id dignissim nunc.
        </p>
      </div>
      <div class="col-card-group">
        <picture data-aos="fade-up" :data-aos-delay="100" data-aos-duration="">
          <img
            src="@/assets/images/award.png"
            alt="Asia Smart App Award 2018/2019"
            loading="lazy"
          />
        </picture>
        <picture data-aos="fade-up" :data-aos-delay="100">
          <img
            src="@/assets/images/award.png"
            alt="Asia Smart App Award 2018/2019"
            loading="lazy"
          />
        </picture>
        <picture data-aos="fade-up">
          <img
            src="@/assets/images/award.png"
            alt="Asia Smart App Award 2018/2019"
            loading="lazy"
          />
        </picture>
        <picture data-aos="fade-up">
          <img
            src="@/assets/images/award.png"
            alt="Asia Smart App Award 2018/2019"
            loading="lazy"
          />
        </picture>
      </div>
    </div>
  </section>
</template>

<script setup>
import TitleComp from '@/components/TitleComp.vue'
</script>

<style lang="scss" scoped>
@import '@/assets/sass/utils/variables';
@import '@/assets/sass/mixins/breakpoint';

section {
  position: relative;
  padding-left: calc($grid-gutter-width / 2);
  @include media-breakpoint-up(md) {
    padding-left: 70px;
  }
  @include media-breakpoint-up(lg) {
    padding-left: calc((100vw - 1240px) / 2);
  }
  &::before {
    @include beforeafter;
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 50%;
    background-color: $primary;
    border-top-left-radius: 30px;
    z-index: -1;
    @include media-breakpoint-up(sm) {
      border-top-left-radius: 50px;
    }
  }
}
.container-fluid {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  padding-top: 65px;
  padding-bottom: 65px;
  background-color: $white;
  border-top-left-radius: 30px;
  border-bottom-left-radius: 30px;
  border-bottom-right-radius: 30px;
  @include media-breakpoint-up(sm) {
    border-top-left-radius: 50px;
    border-bottom-left-radius: 50px;
    border-bottom-right-radius: 50px;
  }
  @include media-breakpoint-up(md) {
    padding-left: 40px;
    padding-right: 40px;
  }
  @include media-breakpoint-up(xl) {
    padding-left: 70px;
    padding-right: calc(((100vw - 1240px) / 2) + 70px);
  }
}
p {
  margin-top: 30px;
  margin-bottom: 20px;
  color: #262626;
  letter-spacing: 0.0625em;
  line-height: 1.75;
}
.col-text {
  @include media-breakpoint-up(md) {
    width: 40%;
  }
  @include media-breakpoint-up(lg) {
    width: 416px;
  }
}
.col-card-group {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  @include media-breakpoint-up(sm) {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
  }
  @include media-breakpoint-up(md) {
    grid-template-columns: 1fr 1fr;
    padding-left: 40px;
    width: 60%;
  }
  @include media-breakpoint-up(lg) {
    gap: 20px 40px;
    width: 285px + 285px + 40px + 40px;
  }
  > * {
    display: table;
  }
  img {
    width: calc(50vw - 40px);
    @include media-breakpoint-up(sm) {
      width: 100%;
    }
    @include media-breakpoint-up(lg) {
      width: 285px;
    }
  }
}
</style>
