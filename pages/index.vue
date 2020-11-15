<template>
  <div class="overflow-hidden">
    <div class="relative lg:pb-0 awal">
      <div class="mx-10 lg:mx-24">
        <Navbar />
        <HeroSection />
      </div>
      <img
        src="~/assets/images/wave.png"
        alt="wave"
        class="hidden lg:block wave"
      />
    </div>
    <!-- Service Section -->
    <ServiceSection />

    <!-- Anak kecil lompat seneng heyy Section -->
    <div class="relative hidden pb-64 mt-20 childern-happy lg:block">
      <div class="flex">
        <div>
          <img
            src="~/assets/images/kids_jump.png"
            alt="kids jump"
            class="-mt-16"
          />
        </div>
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
    <!-- Mobile version -->
    <div class="relative block py-10 mt-10 childern-happy-mobile lg:hidden">
      <div class="flex flex-col mx-10">
        <h1 class="mt-5 text-2xl font-bold text-center text-white">
          Berkembang bersama
        </h1>
        <div class="relative flex flex-row">
          <img
            src="~assets/images/shapes/dots.png"
            class="absolute dots"
            alt=""
          />
          <!-- <img
            src="~/assets/images/kids_jump.png"
            alt="kids jump"
            class="z-10 block -mt-10 -ml-20 sm:hidden"
          /> -->
          <div class="mt-10">
            <p class="text-sm text-justify text-white">
              Di kelaskita. Kami sangat fokus terhadap anak - anak yang sedang
              menuju ke dewasa agar memiliki creativitas, yang dimana di sekolah
              anak - anak jarang di asah creativitasnya, dan disinilah kami
              hadir agar membantu mengembangkan anak yang creative dan inofatif
              kedepannya.
            </p>
            <div class="flex flex-row items-center mt-16">
              <a href="#" class="mr-3 -mt-1 text-base text-white"
                >Tentang Kita
              </a>
              <svg
                width="30"
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
                <rect
                  y="13.4265"
                  width="43.6364"
                  height="1.67832"
                  fill="white"
                />
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
    </div>

    <!-- Mockup Section -->
    <div class="relative pb-64 mt-24 mockup">
      <div class="flex flex-col justify-center mx-10">
        <h1 class="mb-12 text-2xl font-bold text-center lg:text-5xl">
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
    <div class="relative pb-64 testi">
      <div class="mx-5 lg:mx-24">
        <h1 class="mb-12 text-2xl font-bold text-center lg:text-5xl">
          Apa Yang Mereka Katakan
        </h1>
        <!-- Desktop Ver -->
        <div class="hidden lg:block">
          <div class="flex justify-center mt-48">
            <CardTestimoni />
          </div>
          <div class="flex justify-between mt-32">
            <CardTestimoni class="mt-20" />
            <CardTestimoni />
          </div>
        </div>
        <!-- Mobile Ver -->
        <div
          id="card-testi-wrap"
          class="grid grid-flow-col gap-6 ml-8 overflow-scroll lg:hidden card-testi-wrap"
        >
          <CardTestimoni />
          <CardTestimoni />
          <CardTestimoni />
        </div>
        <div class="flex flex-row justify-center mt-10">
          <div @click="left" class="cursor-pointer lg:hidden">
            <svg
              width="50"
              height="50"
              viewBox="0 0 24 24"
              fill="none"
              class="p-3 border rounded-full"
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
              width="50"
              height="50"
              viewBox="0 0 24 24"
              fill="none"
              class="p-3 ml-2 border rounded-full"
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
      </div>
    </div>

    <!-- Footer Section -->
    <Footer />
  </div>
</template>

<script>
export default {
  methods: {
    right() {
      var wrap = document.getElementById("card-testi-wrap");
      wrap.scrollLeft += 330;
    },
    left() {
      var wrap = document.getElementById("card-testi-wrap");
      wrap.scrollLeft -= 330;
    },
  },
};
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
@screen lg {
  .service {
    background-size: 100px;
  }
}
.service {
  background-image: url("~assets/images/shapes/ellips.svg");
  background-repeat: no-repeat;
  background-position: right 30px;
  background-size: 400px;
}

.dots {
  z-index: 1;
  width: 50%;
  top: 80%;
  left: 50%;
}

.childern-happy {
  background-image: url("~assets/images/bg_wave_merah.png");
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  height: 100%;
}

.childern-happy-mobile {
  background-color: #FF7C6D;
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

.card-testi-wrap {
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
