<template>
  <div class="container ">
  <div class="register w-full max-w-xs ">
    <div class="register__content justify-center flex flex-col w-full h-full px-4">
      <div class="register__user flex-col flex">
        <label for="user" class="login__text font-bold text-sm my-2">Nombre</label>
        <input type="text" placeholder="Ingresa tu nombre" id="user" class="login__input shadow appearance-none border rounded-lg py-2 px-3">
      </div>

      <div class="register__user flex-col flex">
        <label for="lastname" class="login__text font-bold text-sm my-2">Apellido</label>
        <input type="text" placeholder="Ingresa tu apellidos" id="lastname" class="login__input shadow appearance-none border rounded-lg py-2 px-3">
      </div>

      <div class="register__user flex-col flex">
        <label for="dni" class="login__text font-bold text-sm my-2">DNI</label>
        <input type="text" placeholder="Ingresa tu DNI" id="dni" class="login__input shadow appearance-none border rounded-lg py-2 px-3">
      </div>

      <div class="register__user flex-col flex">
        <label for="email" class="login__text font-bold text-sm my-2">Correo</label>
        <input type="text" placeholder="Ingresa un correo " id="email" class="login__input shadow appearance-none border rounded-lg py-2 px-3">
      </div>

      <div class="register__user flex-col flex">
        <label for="password" class="login__text font-bold text-sm my-2">Contraseña</label>
        <input type="text" placeholder="Ingresa una contraseña" id="password" class="login__input shadow appearance-none border rounded-lg py-2 px-3">
      </div>
      <div class="register__user flex-col flex">
        <label for="fecha" class="login__text font-bold text-sm my-2">Fecha de Nacimiento</label>
        <input type="text" placeholder="Dia-Mes-Año" id="fecha" class="login__input shadow appearance-none border rounded-lg py-2 px-3">
      </div>
      <div class="register__user flex-col flex">
        <label for="grado" class="login__text font-bold text-sm my-2">Nivel de Estudio</label>
        <input type="text" placeholder="Ingresa tu nivel de estudio" id="grado" class="login__input shadow appearance-none border rounded-lg py-2 px-3">
      </div>

      <div class="register__username flex-col flex">
        <label for="centro" class="login__text font-bold text-sm my-2">Centro de Estudios</label>
        <input type="text" placeholder="Ingrese su centro de estudios" id="centro" class="login__input shadow appearance-none border rounded-lg py-2 px-3">
      </div>

      <div class="register__username flex-col flex">
        <label for="direccion" class="login__text font-bold text-sm my-2">Direccion</label>
        <input type="text" placeholder="Ingrese su centro de estudios" id="direccion" class="login__input shadow appearance-none border rounded-lg py-2 px-3">
      </div>

      <div class="register__username flex-col flex">
        <label for="categoria" class="login__text font-bold text-sm my-2">Categoria</label>
        <input type="text" placeholder="Ingrese las categorias de su interes" id="categoria" class="login__input shadow appearance-none border rounded-lg py-2 px-3">
      </div>

      <div class="flex justify-center flex-col">
        <button class="bg-blue-light rounded-lg my-6">
          <nuxt-link  to="/inicio" class="uppercase text-white no-underline inline-block w-full h-full px-3 py-4 font-bold">
            Registrar
          </nuxt-link>
        </button>
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
  .register {

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
