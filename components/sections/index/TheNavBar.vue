<template>

  <div id="main-header">
    <a id="site-name" href="#"></a>
    <nav>
      <ul>
        <li><a href="">Inicio</a></li>
        <li><a href="">Mis compras</a></li>
        <li><a href="">Mis ventas</a></li>
        <li><a href="/login" >Login</a></li>

      </ul>
    </nav>
  </div>
</template>

<script>
  export default {

  }
</script>

<style scoped lang="scss">
  #main-header {
    background: #333;
    color: white;
    height: 40px;
    width: 100%;
    left: 0;
    top: 0;
    position: fixed;
    a {
      color: white;
    }
  }

  nav {
    float: right;
    ul {
      margin: 0;
      list-style: none;
      padding-right: 10px;
      li {
        display: inline-block;
        line-height: 40px;
        a {
          display: block;
          padding: 0 10px;
          text-decoration: none;
          &:hover {
            background: #0b76a6;
          }
        }
      }
    }
  }
</style>
