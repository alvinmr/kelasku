<template>
  <div
    class="flex items-center content-center justify-between grid-flow-col pt-10 lg:grid lg:justify-between"
  >
    <div class="hidden grid-flow-col gap-10 lg:grid">
      <nuxt-link to="/" class="nav-link">Beranda</nuxt-link>
      <nuxt-link to="tentang" class="nav-link">Tentang Kita</nuxt-link>
    </div>

    <img src="~/assets/images/logo_kelasku.svg" alt="Logo Kelasku" />

    <div class="hidden grid-flow-col gap-10 lg:grid">
      <nuxt-link to="masuk" class="self-center nav-link">Masuk</nuxt-link>
      <nuxt-link to="daftar" class="btn-primary nav-link">Daftar</nuxt-link>
    </div>
    <div class="flex justify-end lg:hidden">
      <svg
        width="50"
        height="50"
        viewBox="0 0 24 24"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <line
          x1="5"
          y1="7"
          x2="19"
          y2="7"
          stroke="#000"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        ></line>
        <line
          x1="5"
          y1="12"
          x2="19"
          y2="12"
          stroke="#000"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        ></line>
        <line
          x1="5"
          y1="17"
          x2="19"
          y2="17"
          stroke="#000"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        ></line>
      </svg>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.nav-link {
  font-family: "Quicksand";
  font-weight: 700;
}

.btn-primary {
  @apply px-8 py-2 text-white bg-blue-500 rounded-full;
}
</style>