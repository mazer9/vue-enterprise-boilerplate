<script>
import NavBar from '@components/nav-bar.vue'

export default {
  components: { NavBar },
}
</script>

<template>
  <div :class="$style.container">
    <NavBar />
    <slot />
  </div>
</template>

<style lang="scss" module>
@import '@design';

.container {
  min-width: $size-content-width-min;
  max-width: $size-content-width-max;
  padding: 0 15px;
  margin: 0 auto;
}
</style>
