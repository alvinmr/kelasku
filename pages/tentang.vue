<template>
  <div class="tentang">
    <div class="mx-24">
      <Navbar />

      <div class="flex flex-row items-center mt-20">
        <div class="w-7/12 p-10">
          <h1 class="text-5xl font-bold">Kelasku</h1>
          <p>
            Di kelaskita. Kami sangat fokus terhadap anak - anak yang sedang
            menuju ke dewasa agar memiliki creativitas, yang dimana di sekolah
            anak - anak jarang di asah creativitasnya, dan disinilah kami hadir
            agar membantu mengembangkan anak yang creative dan inofatif
            kedepannya.
          </p>
        </div>
        <div class="relative w-7/12 tentang-gambar">
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
    <ServiceSection class="mt-40" />
    <Footer />
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.tentang {
  background-color: #F1F1F1;
  height: 100vh;
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