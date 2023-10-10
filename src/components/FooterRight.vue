<script>
import footerRight from '../data/footerRight';

export default {
  name: 'FooterRight',

  data () {
    return {
      footerRight

    }
  }  
}
</script>

<template>
  
  <div class="social">
    <span>Trovaci anche su</span>
    <nav>
      <ul class="flex">
        <li v-for="(item, index) in footerRight" :key="index"><a :href="item.href" target="_blank"><i :class="item.iconClass"></i></a></li>
      </ul>
    </nav>

  </div>
  
</template>

<style lang="scss" scoped>

footer .social {
  span {
    margin: 0 5px;
  }

  a {
    font-size: 1rem;
  }

  * {
    margin-top: 10px;
    margin-bottom: 10px;
  }
} 

</style>