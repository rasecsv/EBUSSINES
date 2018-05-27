<template>
  <div class="index">
    <TheNavBar/>
    <TheSlide/>
    <div class="contenedor">
      <a>hola</a>
    </div>
  </div>


</template>

<script>
import TheNavBar from '../components/sections/index/TheNavBar'
import TheSlide from '../components/sections/index/TheSlide'


export default {
  components: {
    TheSlide,

    TheNavBar

  }
}
</script >

<style lang="scss" scoped>
 .contenedor{
   position: absolute;
   display: flex;
   justify-content: center;
   align-items: center;
   text-align: center;
   margin: 460px auto;

 }
</style>
