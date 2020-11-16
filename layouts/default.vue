<template>
  <div>
    <Nuxt />
  </div>
</template>

<script>
export default {
  transitions: "home",
};
</script>

<style>
.home-enter-active,
.home-leave-active {
  transition: opacity 0.5s;
}
.home-enter,
.home-leave-active {
  opacity: 0;
}
</style>
