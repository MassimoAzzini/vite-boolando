<script>
import footerLeft from '../../data/footerLeft';

export default {
  name: 'FooterLeft',
  data (){
    return {
      footerLeft
    }

  }
  
}
</script>

<template>

  <div class="company">
    <span>Booleando s.r.l.</span>
    <nav>
      <ul class="flex">
        <li v-for="(item, index) in footerLeft" :key="index"><a :href="item.href" target="_self">{{ item.text }}</a></li>
      </ul>
    </nav>
  </div>

  
</template>

<style lang="scss" scoped>

footer .company {
  span {
    font-weight: bold;
    font-size: 1rem;
    margin: 0 5px;
  }

  * {
    margin-top: 10px;
    margin-bottom: 10px;
  }
}

</style>