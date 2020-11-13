<template>
  <div>
    <div class="awal">
      <div class="mx-24">
        <Navbar />
        <HeroSection />
      </div>
      <img src="~/assets/images/wave.png" alt="wave" class="wave" />
    </div>
    <!-- Service Section -->
    <ServiceSection />

    <!-- Anak kecil lompat seneng heyy Section -->
    <div class="relative pb-64 childern-happy">
      <div class="flex">
        <img
          src="~/assets/images/kids_jump.png"
          alt="kids jump"
          class="-mt-16"
        />
        <div class="self-center">
          <h1 class="text-5xl font-bold text-white">Berkembang bersama</h1>
          <p class="w-11/12 mt-5 text-2xl text-white">
            Di kelaskita. Kami sangat fokus terhadap anak - anak yang sedang
            menuju ke dewasa agar memiliki creativitas, yang dimana di sekolah
            anak - anak jarang di asah creativitasnya, dan disinilah kami hadir
            agar membantu mengembangkan anak yang creative dan inofatif
            kedepannya.
          </p>
          <div class="flex flex-row items-center mt-16">
            <a href="#" class="mr-3 -mt-1 text-2xl text-white">Tentang Kita </a>
            <svg
              width="57"
              height="29"
              viewBox="0 0 57 29"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <g clip-path="url(#clip0)">
                <path
                  d="M44.0767 8.40379L42.8761 9.60437L46.832 13.5603L32.9173 13.5603L32.9173 15.2531L46.832 15.2531L42.8761 19.209L44.0767 20.4096L50.0796 14.4067L44.0767 8.40379Z"
                  fill="white"
                />
              </g>
              <rect y="13.4265" width="43.6364" height="1.67832" fill="white" />
              <defs>
                <clipPath id="clip0">
                  <rect
                    width="20.3745"
                    height="20.3745"
                    fill="white"
                    transform="translate(41.6757) rotate(45)"
                  />
                </clipPath>
              </defs>
            </svg>
          </div>
        </div>
      </div>
    </div>

    <!-- Mockup Section -->
    <div class="relative pb-64 mockup">
      <div class="flex flex-col justify-center">
        <h1 class="mb-12 text-5xl font-bold text-center">
          Tersedia di Berbagai Device
        </h1>
        <div class="w-full">
          <img
            src="~assets/images/mockup.png"
            class="mockup-gambar"
            alt="mockup"
          />
        </div>
      </div>
    </div>

    <!-- Testi Section -->
    <div class="relative py-64 testi">
      <div class="mx-24">
        <h1 class="mb-12 text-5xl font-bold text-center">
          Apa Yang Mereka Katakan
        </h1>
        <div>
          <div class="flex justify-center mt-48">
            <CardTestimoni />
          </div>
          <div class="flex justify-between mt-32">
            <CardTestimoni class="mt-20" />
            <CardTestimoni />
          </div>
        </div>
      </div>
    </div>

    <!-- Footer Section -->
    <Footer />
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
  background-size: cover;
}

.wave {
  margin-top: -100px;
}

.service {
  background-image: url("~assets/images/shapes/ellips.svg");
  background-repeat: no-repeat;
  background-position: right;
}

.childern-happy {
  background-image: url("~assets/images/bg_wave_merah.png");
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  height: 100%;
}

.mockup {
  background-image: url("~assets/images/shapes/ellips2.svg");
  background-repeat: no-repeat;
  background-position: left;
}

.mockup-gambar {
  margin-left: 60%;
  transform: translate(-50%);
}

.testi {
  background-image: url("~assets/images/shapes/ellips2.svg");
  background-repeat: no-repeat;
  background-position: 800px 120px;
}

.footer {
  background-image: url("~assets/images/bg_wave_hitam.png");
  background-repeat: no-repeat;
  background-position: bottom;
  background-size: cover;
}
</style>
