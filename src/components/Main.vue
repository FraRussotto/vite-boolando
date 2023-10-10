<script>
  export default{
    name: 'Main'
  }
</script>

<template>
  <main>
    <div class="main_wrapper container">
      <div class="row row-cols-3">

        <div class="col">
          <div class="card">

            <div class="card_image">
              <img src="../asset/img/1.webp" alt="">
            </div>
            <div class="card_text">
              <span class="brand">Guess</span>
              <span class="model">roses tee</span>
              <span class="price">20,99 &euro;</span><span class="oldprice">29,99 &euro;</span>
            </div>

            </div>
          </div>

        <div class="col">
          <div class="card">

            <div class="card_image">
              <img src="../asset/img/1.webp" alt="">
            </div>
            <div class="card_text">
              <span class="brand">Guess</span>
              <span class="model">roses tee</span>
              <span class="price">20,99 &euro;</span><span class="oldprice">29,99 &euro;</span>
            </div>

            </div>
          </div>

        <div class="col">
          <div class="card">

            <div class="card_image">
              <img src="../asset/img/1.webp" alt="">
            </div>
            <div class="card_text">
              <span class="brand">Guess</span>
              <span class="model">roses tee</span>
              <span class="price">20,99 &euro;</span><span class="oldprice">29,99 &euro;</span>
            </div>

            </div>
          </div>

        <div class="col">
          <div class="card">

            <div class="card_image">
              <img src="../asset/img/1.webp" alt="">
            </div>
            <div class="card_text">
              <span class="brand">Guess</span>
              <span class="model">roses tee</span>
              <span class="price">20,99 &euro;</span><span class="oldprice">29,99 &euro;</span>
            </div>

            </div>
          </div>

        <div class="col">
          <div class="card">

            <div class="card_image">
              <img src="../asset/img/1.webp" alt="">
            </div>
            <div class="card_text">
              <span class="brand">Guess</span>
              <span class="model">roses tee</span>
              <span class="price">20,99 &euro;</span><span class="oldprice">29,99 &euro;</span>
            </div>

            </div>
          </div>

        <div class="col">
          <div class="card">

            <div class="card_image">
              <img src="../asset/img/1.webp" alt="">
            </div>
            <div class="card_text">
              <span class="brand">Guess</span>
              <span class="model">roses tee</span>
              <span class="price">20,99 &euro;</span><span class="oldprice">29,99 &euro;</span>
            </div>

            </div>
          </div>

        </div>

      </div>
  </main>

</template>

<style lang="scss">

@use '../scss/partials/variables' as *;

  .card{
    min-width: 250px;
    margin-bottom: 30px;
    border-radius: 0;
    border: 0;
    .card_image{
      img{
        width: 100%;
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