<template>
  <div class="relative flex flex-col">
    <div class="pb-64 service">
      <h1 class="mt-16 text-3xl font-bold text-center lg:text-5xl">
        Kelasku Menyediakan
      </h1>
      <div class="flex mx-auto">
        <div class="flex items-center ml-20">
          <div @click="left" class="cursor-pointer lg:hidden">
            <svg
              width="30"
              height="30"
              viewBox="0 0 24 24"
              fill="none"
              class="p-1 border rounded-full"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M16 4L8 12L16 20"
                stroke="#000"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </svg>
          </div>
          <div @click="right" class="cursor-pointer lg:hidden">
            <svg
              width="30"
              height="30"
              viewBox="0 0 24 24"
              fill="none"
              class="p-1 ml-2 border rounded-full"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M8 4L16 12L8 20"
                stroke="#000"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </svg>
          </div>
        </div>
        <div
          id="card-wrap"
          class="grid justify-start grid-flow-col ml-8 overflow-scroll card-wrap lg:overflow-visible lg:justify-center"
        >
          <CardService
            title="Ebook"
            details="Menyediakan buku creative untuk anak yang tersedia secara gratis dan bisa dibaca kapan pun dan dimana pun."
            :gambar="require('@/assets/images/ebook.svg')"
          />
          <CardService
            class="lg:mt-16"
            title="Video Kreatif"
            details="Selain Ebook gratis kita menyediakan Video yang memacu creativitas anak."
            :gambar="require('@/assets/images/vcreative.svg')"
          />
          <CardService
            title="Teman Diskusi"
            details="Kita akan membantu mengembangkan ide dari anak."
            :gambar="require('@/assets/images/teman_diskusi.svg')"
          />
          <CardService
            class="lg:mt-16"
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
export default {
  methods: {
    right() {
      var wrap = document.getElementById("card-wrap");
      wrap.scrollLeft += 280;
    },
    left() {
      var wrap = document.getElementById("card-wrap");
      wrap.scrollLeft -= 280;
    },
  },
};
</script>

<style>
.card-wrap {
  transition: 0.5s ease-in-out;
  scroll-behavior: smooth;
  -ms-overflow-style: none;
  /* Hides the scrollbar. */

  -ms-scroll-chaining: none;
  /* Prevents Metro from swiping to the next tab or app. */

  -ms-scroll-snap-type: mandatory;
  /* Forces a snap scroll behavior on your images. */

  -ms-scroll-snap-points-x: snapInterval(0%, 100%);
  /* Defines the y and x intervals to snap to when scrolling. */
}
</style>