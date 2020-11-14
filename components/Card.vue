<template>
  <div>
    <div class="flex flex-col p-8 border border-black rounded-xl">
      <div class="bg-black card-image rounded-xl"></div>
      <h1 class="mt-5 text-2xl">Heii ini judul</h1>
      <h1 v-if="hasTime" class="my-3 text-gray-600">Selasa 11.00 - 12.00</h1>
      <div v-if="hasDownloadButton">
        <div class="flex mt-5 cursor-pointer">
          <p class="btn-download hover:bg-blue-100">
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
  </div>
</template>
<script>
export default {
  props: {
    hasTime: Boolean,
    hasDownloadButton: Boolean,
    hasAvatar: Boolean,
    time: String,
    title: String,
    image: String,
  },
};
</script>

<style>
h1 {
  font-family: "Quicksand";
}

.btn-download {
  transition: 0.3s ease-in-out;
  @apply flex flex-row px-5 py-2 text-blue-700
    bg-blue-200;
}

.card-image {
  width: 300px;
  height: 200px;
  background-image: url("https://images.unsplash.com/photo-1593642632823-8f785ba67e45?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=889&q=80");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
</style>