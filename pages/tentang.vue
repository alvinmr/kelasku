<template>
  <div class="tentang">
    <div class="mx-10 lg:mx-24">
      <Navbar />
      <div class="flex flex-col items-center mt-20 lg:flex-row">
        <div class="lg:p-10 lg:w-7/12">
          <h1 class="text-5xl font-bold text-center lg:text-left">Kelasku</h1>
          <p class="my-16 lg:my-0">
            Kelasku sangatlah berfokus terhadap perkembangan anak dibidang
            kreatif. Yang dimana kita ketahui layanan edukasi di bidang kreatif
            kita ketahi di Indonesia masih belom ada. Dan disinilah kita hadir,
            yang bercita-cita ingin membantu perkembangan anak sejak dini,
            supaya tidak takut untuk berkarya.
          </p>
        </div>
        <div class="relative lg:w-7/12 tentang-gambar">
          <div class="absolute shape-1">
            <img src="~assets/images/shapes/tentang/Subtract.svg" alt="" />
          </div>
          <img
            src="https://images.pexels.com/photos/4145354/pexels-photo-4145354.jpeg"
            alt="Gambar Anak Kecil Berkerumun"
          />
          <div class="absolute shape-2">
            <svg
              width="58"
              height="57"
              viewBox="0 0 58 57"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              xmlns:xlink="http://www.w3.org/1999/xlink"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M49.3782 0.661299L0.0317761 48.7032C14.0736 59.8429 34.6648 59.1831 47.5324 46.6557C60.3999 34.1283 60.9647 14.1914 49.3782 0.661299Z"
                fill="url(#pattern0)"
              />
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M49.3782 0.661299L0.0317761 48.7032C14.0736 59.8429 34.6648 59.1831 47.5324 46.6557C60.3999 34.1283 60.9647 14.1914 49.3782 0.661299Z"
                fill="#FFC860"
              />
              <defs>
                <pattern
                  id="pattern0"
                  patternContentUnits="objectBoundingBox"
                  width="1"
                  height="1"
                >
                  <use
                    xlink:href="#image0"
                    transform="translate(0 -0.111029) scale(0.000732064 0.00159122)"
                  />
                </pattern>
              </defs>
            </svg>
          </div>
        </div>
      </div>
    </div>
    <ServiceSection class="my-40" />
    <Footer />
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.tentang {
  background-color: #F1F1F1;
  height: 100%;
}

.shape-1 {
  top: -8%;
  left: -5%;
}

.shape-2 {
  right: -5%;
  bottom: -5%;
}
</style>