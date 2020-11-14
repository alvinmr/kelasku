<template>
  <div>
    <div class="flex items-center justify-center masuk">
      <div class="p-8 my-10 bg-white rounded-xl card-masuk">
        <h1 class="text-4xl font-bold text-center">Kelasku</h1>
        <h3 class="my-10 text-2xl font-bold">Selamat datang kembali</h3>
        <div class="flex flex-col">
          <div class="input-group">
            <label for="email">Email</label>
            <input class="form-input" type="email" name="email" />
          </div>
          <div class="input-group">
            <label for="password">Password</label>
            <input class="form-input" type="password" name="password" />
            <small>8+ karakter</small>
          </div>

          <nuxt-link to="dashboard" class="form-button">Masuk</nuxt-link>
        </div>
        <div class="my-16 bg-black line"></div>
        <div class="flex justify-center -mt-20">
          <p class="px-5 bg-white">atau</p>
        </div>

        <div
          class="flex flex-row justify-center mt-10 cursor-pointer btn-google"
        >
          <div class="flex">
            <img src="~assets/images/google.svg" alt="Google" />
            <h1 class="py-4 text-center">Masuk dengan Google</h1>
          </div>
        </div>
        <div class="flex flex-row justify-center mt-10 asking">
          <h3>Belom punya akun ?</h3>
          <nuxt-link class="ml-2 text-blue-500" to="daftar">Daftar</nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.masuk {
  background-image: url("~assets/images/daftar.jpg");
}
.card-masuk {
  width: 540px;
}
</style>