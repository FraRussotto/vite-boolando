<script>
  export default{
    name: 'Header'
  }
</script>

<template>
  <header>
    <div class="top_bar container">

      <div class="nav_left">
      <ul class="menu_gen">
        <li>
          <a href="#">Uomo</a>
        </li>
        <li>
          <a href="#">Donna</a>
        </li>
        <li>
          <a href="#">Bambino</a>
        </li>
      </ul>
      </div>

      <div class="logo">
      <img src="/boolean-logo.png" alt="">
      </div>

      <div class="nav_right">
      <ul class="menu_account">
        <li>
          <a href="#">Link</a>
        </li>
        <li>
          <a href="#">Link</a>
        </li>
        <li>
          <a href="#">Link</a>
        </li>
      </ul>

      </div>

    </div>
  </header>
</template>

<style lang="scss">

@use '../scss/partials/variables' as *;

header{
  background-color: $primary-color;
  margin-bottom: 40px;
  
  .top_bar{
    height: 50px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    align-items: center;
    .menu_gen{
      display: flex;
      padding: 0;
      li{
        text-transform: capitalize;
        margin-right: 10px;
      }
    }
    img{
      height: 30px;
    }
    .menu_account{
      display: flex;
      li{
        margin-left: 10px;
      }
    }
  }

}

</style>