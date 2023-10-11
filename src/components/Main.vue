<script>
  import ProductCard from './partials/ProductCard.vue';
  import products from '../data/products'

  export default{
    name: 'Main',
    components: {
      ProductCard
    },
    data(){
      return{
        products
      }
    }
  }

</script>

<template>

  <main>

    <div class="main_wrapper container">
      <div class="row row-cols-3">
        <ProductCard  v-for="product in products" 
                      :key="product.id"
                      :marca="product.marca"
                      :modello="product.modello"
                      :price="product.lastPrice"
                      :oldprice="product.fullPrice"
                      />
                      
      </div>
    </div>

  </main>

</template>

<style lang="scss">

@use '../scss/partials/variables' as *;

  main{
    margin-top: 120px;
  }

</style>