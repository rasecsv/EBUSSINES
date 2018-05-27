<template>
  <div class="container">
    <div class="index">
      <TheNavBar/>
    </div>
  <div class="login w-full max-w-xs ">
    <div class="login__content justify-center flex flex-col w-full h-full px-4">

      <div class="login__username flex-col flex">
        <label for="username" class="login__text font-bold text-sm my-2">Username</label>
        <input type="text" placeholder="Ingresa tu usuario..." id="username" class="login__input shadow appearance-none border rounded-lg py-2 px-3">
      </div>
      <div class="login__password flex-col flex">
        <label for="password" class="login__text font-bold text-sm my-2">Password</label>
        <input type="text" placeholder="Ingresa tu contraseña..." id="password" class="login__input shadow appearance-none border rounded-lg py-2 px-3">
      </div>
      <div class="flex justify-center flex-col">
        <button class="bg-blue-light rounded-lg my-6">
          <nuxt-link  to="/inicio" class="uppercase text-white no-underline inline-block w-full h-full px-3 py-4 font-bold">
            Ingresa
          </nuxt-link>
        </button>
        <a class="inline-block align-baseline font-bold text-sm text-blue hover:text-blue-darker text-center" href="/register">Crear Cuenta</a>
      </div>
    </div>
  </div>
  </div>
</template>

<script>
  export default {
    name: 'index'
  }
</script>

<style lang="scss" scoped>
  .login {
    &__text {
      color: #656565;
    }
    &__sub-text {
      color: #B8B8B8;
    }
  }
  .container {
    min-height: 0;
    display: flex;
    justify-content: center;
    align-items: center;
  }

</style>
