<template>
  <div class="flex">
    <div class="side-bar">
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
    <div class="p-16 ml-16 content">
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
  @apply flex flex-col fixed items-center justify-between h-screen p-3;
}
</style>