<template>
  <div>
    <div class="w-full awal">
      <div class="mx-24">
        <Navbar />
        <HeroSection />
      </div>
      <img src="~/assets/images/wave.png" alt="wave" class="wave" />

      <!-- Service Section -->
    </div>
    <div class="pb-64 bg-white service">
      <h1 class="text-3xl font-bold text-center">Kelasku Menyediakan</h1>
      <div class="mx-24">
        <div class="flex">
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
  </div>
</template>

<script>
export default {};
</script>

<style>
* {
  font-family: "Quicksand";
  @apply text-black;
}

.awal {
  height: 100%;
  background-image: url("~assets/images/bg_awan.jpg");
  background-position: center;
  background-repeat: no-repeat;
}

.wave {
  margin-top: -100px;
}

.service {
  background-image: url("~assets/images/shapes/ellips.svg");
  background-repeat: no-repeat;
  background-position: right;
}
</style>
