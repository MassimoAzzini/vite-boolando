<script>
import ProductCard from '../components/partials/ProductCard.vue'
import products from '../data/products';


export default {
  name: 'Main',

  components: {
    ProductCard
  },

  data() {
    return {
      products
    }
  },
  
}
</script>

<template>

  <main>

    <div class="container flex">
      <ProductCard
        v-for="product in products"
        :key="product.id"
        :product="product" />
    </div>

  </main>
  
</template>

<style lang="scss" scoped>

main {
  margin-top: 60px;

  .container {
    padding: 40px 0;
    justify-content: start;
    flex-wrap: wrap;

  }
}

</style>