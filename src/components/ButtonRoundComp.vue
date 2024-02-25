<template>
  <button type="button">
    <slot></slot>
  </button>
</template>

<style lang="scss" scoped>
@import '@/assets/sass/variables';
@import '@/assets/sass/mixins/functions';
button {
  position: relative;
  margin: auto;
  padding: 20px 50px;
  color: $white;
  font-size: $h6;
  font-weight: $font-weight-bold;
  background-color: transparent;
  border: 3px solid $white;
  border-radius: 35px;
  overflow: hidden;
  z-index: 1;
  &::before {
    @include beforeafter;
    position: absolute;
    top: 0;
    left: 0;
    width: 0;
    height: 100%;
    background-color: $lighterBlue;
    transition: width 0.3s;
    z-index: -1;
  }
  &:hover {
    &::before {
      width: 100%;
    }
  }
}
</style>
