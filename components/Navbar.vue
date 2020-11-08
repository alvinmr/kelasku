<template>
  <div
    class="grid items-center content-center justify-between grid-flow-col pt-10"
  >
    <div class="grid grid-flow-col gap-10">
      <a href="#" class="nav-link">Beranda</a>
      <a href="#" class="nav-link">Tentang Kita</a>
    </div>

    <img src="~/assets/images/logo_kelasku.svg" alt="Logo Kelasku" />

    <div class="grid grid-flow-col gap-10">
      <a href="#" class="self-center nav-link">Masuk</a>
      <a href="#" class="btn-primary nav-link">Daftar</a>
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