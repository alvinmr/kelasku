<template>
  <div class="flex justify-center">
    <div
      class="fixed left-0 flex-col items-center justify-between hidden h-screen p-3 side-bar lg:flex"
    >
      <div class="flex mt-10">
        <a href="/dashboard">
          <img
            src="~assets/images/dashboard/home.svg"
            class="placeholder-white via-white"
            alt="Dashboard"
          />
        </a>
      </div>
      <div class="flex flex-col">
        <div class="mb-10 cursor-pointer">
          <img src="~assets/images/dashboard/message.svg" alt="Message" />
        </div>
        <div class="mb-10 cursor-pointer">
          <img
            src="~assets/images/dashboard/bxs-download 2.svg"
            alt="Downloaded"
          />
        </div>
        <div class="mb-10 cursor-pointer">
          <img src="~assets/images/dashboard/bxs-user 2.svg" alt="User" />
        </div>
      </div>
    </div>
    <div class="fixed bottom-0 block w-full bg-blue-900 lg:hidden mobile-bar">
      <div class="flex flex-row justify-around my-5">
        <a href="/dashboard">
          <img
            src="~assets/images/dashboard/home.svg"
            class="placeholder-white via-white"
            alt="Dashboard"
          />
        </a>
        <div class="cursor-pointer">
          <img src="~assets/images/dashboard/message.svg" alt="Message" />
        </div>
        <div class="cursor-pointer">
          <img
            src="~assets/images/dashboard/bxs-download 2.svg"
            alt="Downloaded"
          />
        </div>
        <div class="cursor-pointer">
          <img src="~assets/images/dashboard/bxs-user 2.svg" alt="User" />
        </div>
      </div>
    </div>
    <div class="pb-32 mx-10 mt-10 lg:mx-0 lg:p-16 lg:ml-16 content">
      <Nuxt />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.side-bar {
  width: 5%;
  background-color: #0B1953;
  @apply;
}
</style>