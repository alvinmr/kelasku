<template>
  <div>
    <img src="~assets/images/logo_kelasku.svg" alt="Logo Kelasku" />
    <h1 class="mt-10 text-xl font-bold lg:text-4xl">
      Selamat Datang Di Kelasku
    </h1>
    <div
      class="grid grid-flow-col grid-rows-2 gap-4 lg:grid-rows-none lg:gap-10"
    >
      <MenuDashboard
        title="Ebook"
        :gambar="require('@/assets/images/ebook.svg')"
      />
      <MenuDashboard
        title="Video Creative"
        :gambar="require('@/assets/images/vcreative.svg')"
      />
      <MenuDashboard
        title="Teman Diskusi"
        :gambar="require('@/assets/images/teman_diskusi.svg')"
      />
      <MenuDashboard
        title="Gudang Karya"
        :gambar="require('@/assets/images/gudang_karya.svg')"
      />
    </div>
  </div>
</template>

<script>
export default {
  layout: "dashboard",
};
</script>

<style>
</style>