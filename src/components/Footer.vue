<script>
import FooterLeft from './FooterLeft.vue';
import FooterRight from './FooterRight.vue';

export default {
  name: 'Footer',
  components: {
    FooterLeft,
    FooterRight
  }
  
}
</script>

<template>

  <footer>

    <div class="container flex">

      <FooterLeft />
      
      <FooterRight />

    </div>

  </footer>
  
</template>

<style lang="scss" scoped>

footer {
  background-color: black;
  height: 100px;
  
  .container.flex {
    height: 100%;
    justify-content: space-between;
    align-items: center;
  } 
}

</style>