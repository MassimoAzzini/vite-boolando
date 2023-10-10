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
            <li><a href="#" target="_self"><i class="fa-regular fa-user"></i></a></li>
            <li><a href="#" target="_self"><i class="fa-regular fa-heart"></i></a></li>
            <li><a href="#" target="_self"><i class="fa-solid fa-bag-shopping"></i></a></li>
          </ul>
        </nav>
      </div>
    </div>

  </header>
  
</template>

<style lang="scss" scoped>

header .fixed {
  width: 100%;
  height: 60px;
  background-color: #ff6900;
  box-shadow: 0px 1px 3px grey;
  top: 0;
  z-index: 999;
  }

header .container.flex {
  height: 100%;
  justify-content: space-between;
  align-items: center;
}

header .container .logo {
  width: 120px;
}

</style>