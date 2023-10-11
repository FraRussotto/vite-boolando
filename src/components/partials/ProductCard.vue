<script>
  export default {
    name:'ProductCard',
    props: {
      image: String,
      image_2: String,
      discount: String,
      eco: String,
      marca: String,
      modello: String,
      price: Number,
      oldprice: Number
    }
  }
</script>

<template>

  <div class="col">
    <div class="card">
      <div class="card_image">
        <img :src="image" alt="">
        <img class="secondary-img" :src="image_2" alt="">
        <div class="heart">&hearts;</div>
        <div class="tag">
          <span class="tag_red">{{discount}}</span> <span v-if="!(eco == null)" class="tag_green">{{ eco }}</span>
        </div>
      </div>
      <div class="card_text">
        <span class="brand">{{ marca }}</span>
        <span class="model">{{ modello }}</span>
        <span class="price">{{ price }} &euro;</span> <span v-if="!(oldprice == null)" class="oldprice">{{ oldprice }} &euro;</span>
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
        z-index: 998;
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
        &:hover{
          color: red;
          cursor: pointer;
        }
      }

      .secondary-img{
        position: absolute;
        display: none;
        top: 0;
        left: 0;
      }

      &:hover .secondary-img{
        display: block;
      }

      .tag_red{
        background-color: $badge-color-red;
        color: white;
        font-weight: bold;
        padding: 5px 10px;
      }

      .tag_green{
        background-color: $badge-color-green;
        color: white;
        font-weight: bold;
        padding: 5px 10px;
      }

    }
    .card_text{
      .brand{
        font-size: 0.9rem;
      }
      .model{
        font-size: 1.2rem;
        text-transform: uppercase;
        display: block;
        font-weight: bold;
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