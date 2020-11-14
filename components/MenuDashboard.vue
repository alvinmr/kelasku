<template>
  <div>
    <nuxt-link :to="`dashboard/${title.replace(' ', '-').toLowerCase()}`">
      <div class="menu-dashboard">
        <div class="w-32">
          <img :src="gambar" :alt="title" />
        </div>
        <hr />
        <h1 class="mt-5 text-xl">{{ title }}</h1>
      </div>
    </nuxt-link>
  </div>
</template>

<script>
export default {
  props: {
    gambar: String,
    title: String,
  },
};
</script>

<style>
.menu-dashboard {
  transition: 0.2s ease-in-out;
  background-color: #FBFBFB;
  border: 2px solid #D0D0D0;
  @apply w-64 flex flex-col justify-between mt-10 cursor-pointer rounded-xl p-10 h-56;
}
.menu-dashboard:hover {
  box-shadow: 0px 100px 80px rgba(0, 0, 0, 0.07),
    0px 41.7776px 33.4221px rgba(0, 0, 0, 0.0503198),
    0px 22.3363px 17.869px rgba(0, 0, 0, 0.0417275),
    0px 12.5216px 10.0172px rgba(0, 0, 0, 0.035),
    0px 6.6501px 5.32008px rgba(0, 0, 0, 0.0282725),
    0px 2.76726px 2.21381px rgba(0, 0, 0, 0.0196802);
}
</style>