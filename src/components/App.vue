<script>

  import Header from './Header.vue';
  import Main from './Main.vue';
  import Footer from './Footer.vue';

  export default{
    name: 'App',
    components: {
      Header,
      Main,
      Footer
    }
  }
</script>

<template>
  <Header />
  <Main />
  <Footer />
</template>

<style lang="scss">

@use '../scss/main.scss';

</style>