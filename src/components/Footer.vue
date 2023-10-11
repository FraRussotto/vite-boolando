<<<<<<< HEAD
<script>
  export default{
    name: 'Footer'
  }
</script>

<template>

  <footer>
    <div class="bottom_bar container d-flex justify-content-between align-items-center ">
      <div class="left">
        <h5>Boolando s.r.l.</h5>
        <ul class="p-0 d-flex">
          <li><a href="">Informazioni legali</a></li>
          <li><a href="">Informativa sulla privacy</a></li>
          <li><a href="">Diritto di recesso</a></li>
        </ul>
      </div>
      <div class="right">
        <span>Trovaci anche su</span>
        <ul class="p-0 d-flex justify-content-center">
          <li><a href="">icona</a></li>
          <li><a href="">icona</a></li>
          <li><a href="">icona</a></li>
          <li><a href="">icona</a></li>
          <li><a href="">icona</a></li>
        </ul>
      </div>
    </div>
  </footer>

</template>

<style lang="scss">

@use '../scss/partials/variables' as *;

footer{
  background-color: $footer-bg-color;
  height: 90px;
  color: white;
  padding-top: 15px;
  .bottom_bar{
    height: 100%;
    .left{
    li{
      margin-right: 5px;
      font-size: 0.6rem;
      }
    }
    .right{
    text-align: center;
    span{
      font-size: 0.8rem;
    }
    li{
      margin-left: 5px;
      font-size: 0.6rem;
      }
    }
  }
}

=======
<script>
  export default{
    name: 'Footer'
  }
</script>

<template>

  <footer>
    <div class="bottom_bar container d-flex justify-content-between align-items-center ">
      <div class="left">
        <h5>Boolando s.r.l.</h5>
        <ul class="p-0 d-flex">
          <li><a href="">Informazioni legali</a></li>
          <li><a href="">Informativa sulla privacy</a></li>
          <li><a href="">Diritto di recesso</a></li>
        </ul>
      </div>
      <div class="right">
        <span>Trovaci anche su</span>
        <ul class="p-0 d-flex justify-content-center">
          <li><a href="">icona</a></li>
          <li><a href="">icona</a></li>
          <li><a href="">icona</a></li>
          <li><a href="">icona</a></li>
          <li><a href="">icona</a></li>
        </ul>
      </div>
    </div>
  </footer>

</template>

<style lang="scss">

@use '../scss/partials/variables' as *;

footer{
  background-color: $footer-bg-color;
  height: 70px;
  color: white;
  padding-top: 15px;
  .bottom_bar{
    height: 100%;
    .left{
    li{
      margin-right: 5px;
      font-size: 0.6rem;
      }
    }
    .right{
    text-align: center;
    span{
      font-size: 0.8rem;
    }
    li{
      margin-left: 5px;
      font-size: 0.6rem;
      }
    }
  }
}

>>>>>>> f9b47561f1d3beb16f947e05d85f31441c0eaadb
</style>