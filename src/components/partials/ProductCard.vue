<script>
export default {
  name: 'ProductCard',

  props: {
    product: Object
  },

  data() {
    return {
      isActive: false
    }
  },

  methods: {
    getImagePath(img){
      return new URL(`/src/assets/img/${img}`, import.meta.url).href;
    }
  },

}

</script>

<template>

  <div class="product" @click="isActive = !isActive">
    <div class="image relative">
      <img id="img-relaxed" :src="getImagePath(product.primaryImage)" alt="">
      <img class="secondary-image" :src="getImagePath(product.secondaryImage)" alt="">
      <span class="heart" :class="{active : isActive}"><i class="fa-solid fa-heart"></i></span>
      <div class="tag">
        <span v-if="product.discount" class="discount">{{product.discount}}</span>
        <span v-if="product.sostenibilita" class="sostenibilita">Sostenibilita</span>
      </div>
    </div>
    <div class="description">
      <span class="marca">{{product.marca}}</span>
      <span class="modello">{{product.modello}}</span>
      <div class="price">
        <span class="last-price">{{product.lastPrice}}</span>
        <span class="full-price">{{product.fullPrice}}</span>
      </div>
    </div>
  </div>

  
</template>

<style lang="scss" scoped>

.active {
  color: red;
}

.product {
  max-width: 400px;
  width: calc(100% / 3);
  min-width: 250px;
  padding: 5px;

  .image{

    img {
      width: 100%;
    }

    .secondary-image {
      position: absolute;
      top: 0;
      left: 0;
      display: none;
    }

    .heart {
      cursor: pointer;
      position: absolute;
      right: 0;
      top: 10px;
      background-color: white;
      padding: 10px;
      &:hover {
        color: red;
      }
    }

    .tag {
      position: absolute;
      left: 0;
      bottom: 40px;
      font-size: 0.7rem;
      color: white;

      .discount {
        background-color: red;
        padding: 5px 10px;

        .d-none {
          display: none;
        }
      }

      .sostenibilita {
        background-color: green;
        padding: 5px 10px;
      }
    }

    &:hover .secondary-image {
      display: block;
    }
  }

  .description {

    .marca,
    .modello {
      display: block;
    }

    .modello {
      font-weight: bold;
    }

    .price {
      font-size: 0.8rem;

      .last-price {
        color: red;
        font-weight: bold;
        margin-right: 5px;
      }

      .full-price {
        text-decoration: line-through;
      }
    }
  }
}

</style>