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
      <ul>
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
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 999;
  
  .top_bar{
    height: 80px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    .nav_left{
      flex-basis: 30%;
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
    }
    .logo{
      flex-basis: 100%;
      text-align: center;
      img{
        height: 50px;
      }
    }
    .nav_right{
      display: flex;
      justify-content: flex-end;
      flex-basis: 30%;
      ul{
        display: flex;
        padding: 0;
        margin-bottom: 0;
        li{
          a{
            margin-left: 10px;
          }
        }
      }
    }
  }

}
</style>
