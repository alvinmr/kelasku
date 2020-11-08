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
    <div class="pb-64 bg-white">
      <h1 class="text-3xl font-bold text-center">Kelasku Menyediakan</h1>
      <div class="mx-24">
        <div class="flex">
          <CardService />
          <CardService class="mt-16" />
          <CardService />
          <CardService class="mt-16" />
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
</style>
