<template>
  <div class="contenedor">
    <div class="outer-wrapper ">
      <div class="s-wrap s-type-2" role="slider">
        <ul class="s-content">
          <li class="s-item s-item-1"></li>
          <li class="s-item s-item-2"></li>
          <li class="s-item s-item-3"></li>
          <li class="s-item s-item-4"></li>
          <li class="s-item s-item-5"></li>
        </ul>
      </div>
    </div>
  </div>

</template>

<script>
  export default {
    name: 'TheSlide'
  }
</script>

<style lang="scss" scoped>
  .contenedor {
    position: absolute;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    margin: 40px auto;


  }
  $switch-speed: 1s;
  $slider-number: 5;
  $slider-width: 100% / $slider-number;

  $image1: 'https://images.unsplash.com/photo-1457369804613-52c61a468e7d?crop=entropy&fit=crop&fm=jpg&h=600&ixjsv=2.1.0&ixlib=rb-0.3.5&q=80&w=800';
  $image2: 'https://images.unsplash.com/photo-1456318019777-ccdc4d5b2396?crop=entropy&fit=crop&fm=jpg&h=600&ixjsv=2.1.0&ixlib=rb-0.3.5&q=80&w=800';
  $image3: 'https://images.unsplash.com/photo-1428189923803-e9801d464d76?crop=entropy&fit=crop&fm=jpg&h=600&ixjsv=2.1.0&ixlib=rb-0.3.5&q=80&w=800';
  $image4: 'https://images.unsplash.com/photo-1422393462206-207b0fbd8d6b?crop=entropy&fit=crop&fm=jpg&h=600&ixjsv=2.1.0&ixlib=rb-0.3.5&q=80&w=800';
  $image5: 'https://images.unsplash.com/photo-1439736637365-748f240b24fb?crop=entropy&fit=crop&fm=jpg&ixjsv=2.1.0&ixlib=rb-0.3.5&q=80&w=800';

  *,
  *::before,
  *::after {
    box-sizing: border-box;
  }


  .outer-wrapper {
    width: 100%;
    height: 400px;
    margin: 0px auto;
  }

  .s-wrap {
    width: 1290px;
    height: 400px;
    margin-bottom: 50px;
    padding-bottom: 55%;
    position: absolute;
    border: 1px solid #fff;
    background-color: #efefe8;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
    overflow: hidden;

    > input {
      display: none;
    }

    .s-content {
      margin: 0;
      padding: 0;
      position: absolute;
      top: 0;
      left: 0;
      width: 100% * $slider-number;
      height: 100%;
      font-size: 0;
      list-style: none;
      transition: transform $switch-speed;
    }

    .s-item {
      display: inline-block;
      width: $slider-width;
      height: 100%;
      background-repeat: no-repeat;
      background-size: cover;
    }

    .s-item-1 {background-image: url($image1);}
    .s-item-2 {background-image: url($image2);}
    .s-item-3 {background-image: url($image3);}
    .s-item-4 {background-image: url($image4);}
    .s-item-5 {background-image: url($image5);}
  }


  .s-type-2 {
    .s-content {
      animation: slider-animation 50s ease-in-out infinite;

      &:hover {animation-play-state: paused;}
    }
  }

  @keyframes slider-animation {
    $i: 0;
    $j: 0;
    $times: ($slider-number - 1) * 2;
    @while $i < 100 {
      #{$i}%,
      #{$i + 7}% {
        @if $i < 50 {
          transform: translateX(-$slider-width * $j);
        } @else {
          transform: translateX(-$slider-width * ($times - $j));
        }
      }

      $i: $i + 100 / $times;
      $j: $j + 1;
    }
  }
</style>
