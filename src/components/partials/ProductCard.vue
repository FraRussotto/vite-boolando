<script>
  export default{
    name:'ProductCard'
  }
</script>

<template>

  <div class="col">
    <div class="card">
      <div class="card_image">
        <img src="../../asset/img/1.webp" alt="">
        <img class="secondary-img" src="../../asset/img/1b.webp" alt="">
        <div class="heart">&hearts;</div>
        <div class="tag">
          <span class="tag_red">-50%</span> <span class="tag_green">Sostenibilità</span>
        </div>
      </div>
      <div class="card_text">
        <span class="brand">Guess</span>
        <span class="model">roses tee</span>
        <span class="price">20,99 &euro;</span><span class="oldprice">29,99 &euro;</span>
      </div>
    </div>
  </div>

</template>

<style lang="scss">

@use '../../scss/partials/variables' as *;

    .card{
    min-width: 250px;
    margin-bottom: 30px;
    .card_image{
      position: relative;
      img{
        width: 100%;
      }
      .tag{
        position: absolute;
        z-index: 999;
        bottom: 20px; 
      }
      .heart{
        position: absolute;
        top: 20px;
        right: 0;
        background-color: white;
        width: 50px;
        height: 50px;
        line-height: 50px;
        vertical-align: center;
        text-align: center;
        font-size: 2.5rem;
      }
      .heart:hover{
        color: red;
        cursor: pointer;
      }

      .secondary-img{
        position: absolute;
        display: none;
        top: 0;
        left: 0;
      }

      .card_image:hover .secondary-img{
        display: block;
      }

      .tag_red{
        background-color: #ff0000;
        color: white;
        font-weight: bold;
        padding: 5px 10px;
      }

      .tag_green{
        background-color: #008000;
        color: white;
        font-weight: bold;
        padding: 5px 10px;
      }

    }
    .card_text{
      .brand{
        font-size: 1.1rem;
      }
      .model{
        font-size: 1.2rem;
        text-transform: uppercase;
        display: block;
      }
      .price{
        color: $badge-color-red;
        font-weight: bold;
      }
      .oldprice{
        text-decoration: line-through;
        margin-left: 5px;
      }
    }
  }

</style>