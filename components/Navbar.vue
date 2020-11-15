<template>
  <div>
    <div
      class="flex items-center content-center justify-between grid-flow-col pt-10 lg:grid lg:justify-between"
    >
      <div class="hidden grid-flow-col gap-10 lg:grid">
        <nuxt-link to="/" class="nav-link">Beranda</nuxt-link>
        <nuxt-link to="tentang" class="nav-link">Tentang Kita</nuxt-link>
      </div>

      <img
        src="~/assets/images/logo_kelasku.svg"
        class="cursor-pointer"
        alt="Logo Kelasku"
      />

      <div class="hidden grid-flow-col gap-10 lg:grid">
        <nuxt-link to="masuk" class="self-center nav-link">Masuk</nuxt-link>
        <nuxt-link to="daftar" class="btn-primary nav-link">Daftar</nuxt-link>
      </div>
      <!-- Nav Hamburger -->
      <div class="flex justify-end lg:hidden">
        <button @click="openNav" class="cursor-pointer nav-toggle">
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
        </button>
      </div>
    </div>

    <div class="hidden p-10 nav-mobile">
      <div class="flex">
        <div class="mx-auto">
          <img
            src="~/assets/images/logo_kelasku.svg"
            class="cursor-pointer"
            alt="Logo Kelasku"
          />
        </div>
        <div @click="closeNav" class="-ml-16 cursor-pointer">
          <svg
            width="50"
            height="50"
            viewBox="0 0 24 24"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M16 8L12 12M12 12L8 16M12 12L8 8M12 12L16 16"
              stroke="#000"
              stroke-width="1.5"
              stroke-linecap="round"
              stroke-linejoin="round"
            ></path>
          </svg>
        </div>
      </div>
      <div class="flex flex-col mt-10">
        <nuxt-link class="mt-10 text-3xl font-bold" to="/">Beranda</nuxt-link>
        <nuxt-link class="mt-10 text-3xl font-bold" to="/tentang"
          >Tentang Kita</nuxt-link
        >
        <nuxt-link class="mt-10 text-3xl font-bold" to="/masuk"
          >Masuk</nuxt-link
        >
        <nuxt-link class="mt-10 text-3xl font-bold" to="/daftar"
          >Daftar</nuxt-link
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isActived: false,
    };
  },
  methods: {
    openNav() {
      var nav = document.querySelector(".nav-mobile");
      nav.classList.replace("hidden", "block");
    },
    closeNav() {
      var nav = document.querySelector(".nav-mobile");
      nav.classList.replace("block", "hidden");
    },
  },
};
</script>

<style>
.nav-link {
  font-family: "Quicksand";
  font-weight: 700;
}

.btn-primary {
  @apply px-8 py-2 text-white bg-blue-500 rounded-full;
}

.nav-mobile {
  transition: 1s linear all;
  @apply fixed z-10 w-screen h-screen bg-white top-0 left-0;
}
</style>