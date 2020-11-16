<template>
  <div>
    <div class="flex flex-col">
      <nuxt-link to="/dashboard" class="flex flex-row">
        <svg
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            class="arrow-back"
            d="M21 12H3M3 12L10 5M3 12L10 19"
            stroke="#000"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          ></path>
        </svg>
        <p class="ml-5 text-gray-600">Kembali ke dashboard</p>
      </nuxt-link>
      <h1 class="mt-5 text-3xl">Video Kreatif</h1>
      <div class="grid gap-10 mt-16 lg:grid-cols-3 md:grid-cols-2">
        <Card
          hasDownloadButton
          title="Susun Dan Implementasikan"
          image="https://raw.githubusercontent.com/alvinmr/kelasku/main/assets/gambar_kelas/video_creativ/1.png"
        />
        <Card
          hasDownloadButton
          title="Jangan Takut Dalam Memulai"
          image="https://raw.githubusercontent.com/alvinmr/kelasku/main/assets/gambar_kelas/video_creativ/2.png"
        />
        <Card
          hasDownloadButton
          title="Hirarki Dalam Desain"
          image="https://raw.githubusercontent.com/alvinmr/kelasku/main/assets/gambar_kelas/video_creativ/3.png"
        />
        <Card
          hasDownloadButton
          title="Apa itu Ide ?"
          image="https://raw.githubusercontent.com/alvinmr/kelasku/main/assets/gambar_kelas/video_creativ/4.png"
        />
        <Card
          hasDownloadButton
          title="Susun Dan Eksekuasi"
          image="https://raw.githubusercontent.com/alvinmr/kelasku/main/assets/gambar_kelas/video_creativ/5.png"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  layout: "dashboard",
};
</script>

<style>
.arrow-back {
  fill: grey;
}
</style>