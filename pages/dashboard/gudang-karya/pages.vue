<template>
  <div>
    <div class="mx-24">
      <nuxt-link to="/dashboard" class="flex flex-row py-10">
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
            stroke="#fff"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          ></path>
        </svg>
        <p class="ml-5 text-gray-200">Kembali ke dashboard</p>
      </nuxt-link>
      <h1 class="mb-5 text-5xl font-bold text-white">Gudang Karya</h1>
    </div>
    <div class="flex flex-row justify-center mx-24">
      <div class="image-page"></div>
      <img src="~assets/images/gudang_karya.png" class="w-full" />
      <div class="flex flex-col w-11/12 ml-5">
        <h1 class="text-3xl font-bold text-white">Hello world</h1>
        <p class="text-xl text-white">
          setiap orang memiliki mimpi yang ingin mereka wujudkan. Namun tidak
          semua orang bisa meraihnya, karena usaha mereka berbeda - beda. Ada
          yang hanya mencapai pada titik terendak, sedangkan bahkan ada yang
          mencapai titil tertinggi dan yang mencapai titip terendah, biasanya
          kerena mereka tidak pernah memulai usaha untuk menggapai mimpinya.
          Sangat disayangkan bukan? Sebagia kaum mileniak muda yang katanya kita
          itu multi talenta, cerdas, kreatif, motivasi, bikin karya apa saja
          pasti bagus, dan usahanya? tidak usah diragukan lagi, kitapun sebagai
          anak muda, haruslah terbang menggapai apa yang kita inginkan.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  layout: "pages",
};
</script>

<style>
.image-page {
  background-image: url("~assets/images/gudang_karya.png");
  background-repeat: no-repeat;
  background-size: cover;
}
</style>