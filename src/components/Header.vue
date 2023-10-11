<script>
  export default{
    name: 'Header'
  }
</script>

<template>
  <header>
    <div class="top_bar container align-items-center ">

      <div class="nav_left">
      <ul>
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
          <a href="#"><i class="fa-regular fa-user"></i></a>
        </li>
        <li>
          <a href="#"><i class="fa-regular fa-heart"></i></a>
        </li>
        <li>
          <a href="#"><i class="fa-solid fa-bag-shopping"></i></a>
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
    height: 80px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    ul{
      display: flex;
      padding: 0;
      margin-bottom: 0;
      li{
        a{
          text-transform: capitalize;
          margin-right: 10px;
          font-weight: bold;
          &:hover{
            text-decoration: underline;
          }
        }
      }
    }
    img{
      height: 50px;
    }
    .menu_account{
      display: flex;
      li{
        a{
          margin-left: 10px;
        }
      }
    }
  }

}
</style>
