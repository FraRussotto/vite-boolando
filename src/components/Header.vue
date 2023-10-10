<script>
  export default{
    name: 'Header'
  }
</script>

<template>
  <header>
    <div class="nav">
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
  </header>
</template>

<style lang="scss">

header{
  height: 80px;
  background-color: $primary-color;
}

img{
  width: 200px;
}

</style>