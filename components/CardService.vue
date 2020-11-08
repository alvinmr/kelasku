<template>
  <div>
    <div class="flex flex-col items-start justify-between p-8 card-service">
      <img :src="gambar" class="" alt="Logo Card Service" />
      <h2 class="text-2xl font-bold">{{ title }}</h2>
      <p class="text-sm">
        {{ details }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    gambar: String,
    details: String,
    title: String,
  },
};
</script>

<style>
.card-service {
  height: 280px;
  width: 250px;
  box-shadow: 0px 100px 80px rgba(0, 0, 0, 0.07),
    0px 41.7776px 33.4221px rgba(0, 0, 0, 0.0503198),
    0px 22.3363px 17.869px rgba(0, 0, 0, 0.0417275),
    0px 12.5216px 10.0172px rgba(0, 0, 0, 0.035),
    0px 6.6501px 5.32008px rgba(0, 0, 0, 0.0282725),
    0px 2.76726px 2.21381px rgba(0, 0, 0, 0.0196802);
  background: #fbfbfb;
  @apply mt-20 mr-12 relative 
    rounded-xl;
}
</style>