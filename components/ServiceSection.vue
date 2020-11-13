<template>
  <div class="pb-64 service">
    <h1 class="text-5xl font-bold text-center">Kelasku Menyediakan</h1>
    <div class="mx-auto">
      <div class="flex justify-center">
        <CardService
          title="Ebook"
          details="Menyediakan buku creative untuk anak yang tersedia secara gratis dan bisa dibaca kapan pun dan dimana pun."
          :gambar="require('@/assets/images/ebook.svg')"
        />
        <CardService
          class="mt-16"
          title="Video Creative"
          details="Selain Ebook gratis kita menyediakan Video yang memacu creativitas anak."
          :gambar="require('@/assets/images/vcreative.svg')"
        />
        <CardService
          title="Teman Diskusi"
          details="Kita akan membantu mengembangkan ide dari anak."
          :gambar="require('@/assets/images/teman_diskusi.svg')"
        />
        <CardService
          class="mt-16"
          title="Gudang Karya"
          details="Berisi beberapa hasil karya dari anak yang sudah mengikuti kelaskita."
          :gambar="require('@/assets/images/gudang_karya.svg')"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>