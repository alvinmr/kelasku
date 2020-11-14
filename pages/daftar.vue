<template>
  <div>
    <div class="flex items-center justify-center daftar">
      <div class="p-8 my-10 bg-white rounded-xl">
        <h1 class="text-4xl font-bold text-center">Kelasku</h1>
        <h3 class="mt-10 text-2xl font-bold">Pendaftaran</h3>
        <p class="mb-10">Lengkapi data pribadi kamu di bawah ini</p>
        <div class="flex flex-col">
          <div class="flex flex-row">
            <div class="mr-2 input-group">
              <label for="nama_depan">Nama depan</label>
              <input type="text" name="nama_depan" />
            </div>
            <div class="input-group">
              <label for="nama_belakang">Nama belakang</label>
              <input type="text" name="nama_belakang" />
            </div>
          </div>
          <div class="input-group">
            <label for="email">Email</label>
            <input type="email" name="email" />
          </div>
          <div class="input-group">
            <label for="password">Password</label>
            <input type="password" name="password" />
            <small>8+ karakter</small>
          </div>

          <nuxt-link to="dashboard" class="form-button">Daftar</nuxt-link>
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
            <h1 class="py-4 text-center">Daftar dengan Google</h1>
          </div>
        </div>
        <div class="flex flex-row justify-center mt-10 asking">
          <h3>Sudah punya akun ?</h3>
          <nuxt-link class="ml-2 text-blue-500" to="masuk">Masuk</nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
input {
  border: 2px solid #F1F1F1;
  height: 50px;
  transition: 0.2s ease-in-out;
  padding: 10px;
}

input:focus {
  border: 2px solid black;
}

.daftar {
  font-family: "Montserrat";
  background-image: url("~assets/images/masuk.jpg");
}

.input-group {
  @apply flex flex-col mt-5;
}

.form-button {
  background-color: #7EA6E0;
  @apply w-full py-4 mt-5 font-bold text-center text-white;
}

.btn-google {
  background-color: #F1F1F1;
}

.line {
  height: 1px;
}

.asking {
  font-family: "Montserrat";
}
</style>