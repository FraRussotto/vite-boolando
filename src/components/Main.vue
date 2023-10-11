<script>
  import ProductCard from './partials/ProductCard.vue';

  export default{
    name: 'Main',
    components: {
    ProductCard,
}
  }
</script>

<template>

  <main>

    <div class="main_wrapper container">
      <div class="row row-cols-3">
        <ProductCard />
        <ProductCard />
        <ProductCard />
        <ProductCard />
        <ProductCard />
        <ProductCard />
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