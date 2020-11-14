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
      <h1 class="mt-5 text-3xl">Ebook</h1>
      <div class="grid grid-cols-3 gap-10 mt-16">
        <Card hasDownloadButton />
        <Card hasDownloadButton />
        <Card hasDownloadButton />
        <Card hasDownloadButton />
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