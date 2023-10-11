<script>
import menuHeader from '../data/menuHeader'
import menuHeaderIcon from '../data/menuHeaderIcon';

export default {
  name: 'Header',
  data() {
    return {
      menuHeader,
      menuHeaderIcon
    }
  },
}

</script>

<template>

  <header>

    <div class="fixed">
      <div class="container flex">

        <nav>
          <ul class="flex">
            <li v-for="(item, index) in menuHeader"
            :key="index"><a :href="item.href" target="_self">{{ item.text }}</a></li>
          </ul>
        </nav>

        <img class="logo" src="../assets/img/boolean-logo.png" alt="Logo">

        <nav>
          <ul class="flex">
            <li v-for="(item, index) in menuHeaderIcon" :key="index">
              <a :href="item.href" target="_self">
                <i :class="item.iconClass"></i>
              </a>
            </li>
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

  .container {
    height: 100%;
    justify-content: space-between;
    align-items: center;

    .logo {
      width: 120px;
    }
  }
}

</style>