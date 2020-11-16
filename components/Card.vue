<template>
  <div>
    <nuxt-link to="/">
      <div class="flex flex-col p-8 border border-black card rounded-xl">
        <div
          :style="{ backgroundImage: 'url(' + require(image) + '))' }"
          class="flex flex-grow bg-black card-image rounded-xl"
        ></div>
        <h1 class="mt-5 text-2xl">{{ title }}</h1>
        <h1 v-if="hasTime" class="my-3 text-gray-600">{{ time }}</h1>
        <div v-if="hasDownloadButton">
          <div class="flex flex-grow mt-5 cursor-pointer">
            <p class="btn-download hover:bg-blue-100 focus:bg-indigo-100">
              <img src="~assets/images/download.svg" class="mr-2" />
              Download
            </p>
          </div>
        </div>
        <div class="mt-5" v-if="hasAvatar">
          <hr />
          <div class="flex flex-row items-center mt-5">
            <img
              src="https://i.pravatar.cc/300"
              class="w-2/12 rounded-full"
              alt="avatar"
            />
            <div class="ml-5">
              <h1>Alvin Maulana</h1>
            </div>
          </div>
        </div>
      </div>
    </nuxt-link>
  </div>
</template>
<script>
export default {
  props: {
    hasTime: Boolean,
    hasDownloadButton: Boolean,
    hasAvatar: Boolean,
    time: {
      type: String,
      default: "Selasa 11.00 - 12.00",
    },
    title: {
      type: String,
      default: "Ini Title bagusss banget",
    },
    image: {
      type: String,
      default: "~assets/gambar_kelas/ebook/1.png",
    },
  },
};
</script>

<style>
h1 {
  font-family: "Quicksand";
}

.card {
  transition: 0.3s linear;
}

.card:hover {
  box-shadow: 0px 100px 80px rgba(0, 0, 0, 0.07),
    0px 41.7776px 33.4221px rgba(0, 0, 0, 0.0503198),
    0px 22.3363px 17.869px rgba(0, 0, 0, 0.0417275),
    0px 12.5216px 10.0172px rgba(0, 0, 0, 0.035),
    0px 6.6501px 5.32008px rgba(0, 0, 0, 0.0282725),
    0px 2.76726px 2.21381px rgba(0, 0, 0, 0.0196802);
}

.btn-download {
  transition: 0.3s ease-in-out;
  @apply flex flex-row px-5 py-2 text-blue-700
    bg-blue-200;
}

.card-image {
  height: 250px;
  /* background-image: url("~assets/gambar_kelas/ebook/1.png"); */
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
</style>