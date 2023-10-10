<script>
export default {
  name: 'Header',
  
}
</script>

<template>

  <header>

    <div class="fixed">
      <div class="container flex">
        <nav>
          <ul class="flex">
            <li><a href="#" target="_self">Donna</a></li>
            <li><a href="#" target="_self">Uomo</a></li>
            <li><a href="#" target="_self">Bambini</a></li>
          </ul>
        </nav>
        <img class="logo" src="../assets/img/boolean-logo.png" alt="Logo">
        <nav>
          <ul class="flex">
            <li><a href="#" target="_self"><font-awesome-icon icon="fa-regular fa-user" /></a></li>
            <li><a href="#" target="_self"><i class="fa-regular fa-heart"></i></a></li>
            <li><a href="#" target="_self"><i class="fa-solid fa-bag-shopping"></i></a></li>
          </ul>
        </nav>
      </div>
    </div>

  </header>
  
</template>

<style lang="scss" scoped>

</style>