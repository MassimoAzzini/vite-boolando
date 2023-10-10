<script>
export default {
  name: 'Main',
  
}
</script>

<template>

  <main>

    <div class="container flex">
      <!-- CARD RELAXED-->
      <div class="product">
        <div class="image relative">
          <img id="img-relaxed" src="../assets/img/1.webp" alt="">
          <img class="secondary-image" src="../assets/img/1b.webp" alt="">
          <span class="heart"><i class="fa-solid fa-heart"></i></span>
          <div class="tag">
            <span class="discount">-50%</span>
            <span class="sostenibilita">Sostenibilità</span>
          </div>
        </div>
        <div class="description">
          <span class="marca">Levi's</span>
          <span class="modello">RELAXED FIT TEE UNISEX</span>
          <div class="price">
            <span class="last-price">14,99 €</span>
            <span class="full-price">29,99 €</span>
          </div>
        </div>
      </div>
      <!-- fine CARD RELAXED-->

      <!-- CARD ROSES -->
      <div class="product">
        <div class="image relative">
          <img id="img-roses" src="../assets/img/2.webp" alt="">
          <img class="secondary-image" src="../assets/img/2b.webp" alt="">
          <span class="heart"><i class="fa-solid fa-heart"></i></span>
          <div class="tag">
            <span class="discount">-30%</span>
            <!-- <span class="sostenibilita">Sostenibilità</span> -->
          </div>
        </div>
        <div class="description">
          <span class="marca">Guess</span>
          <span class="modello">ROSES TEE</span>
          <div class="price">
            <span class="last-price">20,99 €</span>
            <span class="full-price">29,99 €</span>
          </div>
        </div>
      </div>
      <!-- FINE CARD ROSES-->

      <!-- CARD VOGLIA -->
      <div class="product">
        <div class="image relative">
          <img id="img-voglia" src="../assets/img/3.webp" alt="">
          <img class="secondary-image" src="../assets/img/3b.webp" alt="">
          <span class="heart"><i class="fa-solid fa-heart"></i></span>
          <div class="tag">
            <span class="discount">-30%</span>
            <!-- <span class="sostenibilita">Sostenibilità</span> -->
          </div>
        </div>
        <div class="description">
          <span class="marca">Come Zucchero Filato</span>
          <span class="modello">VOGLIA DI COLORI PASTELLO</span>
          <div class="price">
            <span class="last-price">129,99 €</span>
            <span class="full-price">184,99 €</span>
          </div>
        </div>
      </div>
      <!-- FINE CARD VOGLIA-->

      <!-- CARD TEE UNISEX-->
      <div class="product">
        <div class="image relative">
          <img id="img-tee-unisex" src="../assets/img/4.webp" alt="">
          <img class="secondary-image" src="../assets/img/4b.webp" alt="">
          <span class="heart"><i class="fa-solid fa-heart"></i></span>
          <div class="tag">
            <span class="discount">-50%</span>
            <span class="sostenibilita">Sostenibilità</span>
          </div>
        </div>
        <div class="description">
          <span class="marca">Levi's</span>
          <span class="modello">TEE UNISEX</span>
          <div class="price">
            <span class="last-price">14,99 €</span>
            <span class="full-price">29,99 €</span>
          </div>
        </div>
      </div>
      <!-- fine CARD TEE UNISEX-->

      <!-- CARD STRIPE-->
      <div class="product">
        <div class="image relative">
          <img id="img-stripe" src="../assets/img/5.webp" alt="">
          <img class="secondary-image" src="../assets/img/5b.webp" alt="">
          <span class="heart"><i class="fa-solid fa-heart"></i></span>
          <!-- <div class="tag">
            <span class="discount">-50%</span>
            <span class="sostenibilita">Sostenibilità</span>
          </div> -->
        </div> 
        <div class="description">
          <span class="marca">Maya Deluxe</span>
          <span class="modello">STRIPE BODICE</span>
          <div class="price">
            <span class="last-price">99,99 €</span>
            <!-- <span class="full-price"> 99,99 €</span> -->
          </div>
        </div>
      </div>
      <!-- fine CARD STRIPE-->

      <!-- CARD MAGLIONE-->
      <div class="product">
        <div class="image relative">
          <img id="img-maglione" src="../assets/img/6.webp" alt="">
          <img class="secondary-image" src="../assets/img/6b.webp" alt="">
          <span class="heart"><i class="fa-solid fa-heart"></i></span>
          <div class="tag">
            <!-- <span class="discount">-50%</span> -->
            <span class="sostenibilita">Sostenibilità</span>
          </div>
        </div>
        <div class="description">
          <span class="marca">Esprit</span>
          <span class="modello">MAGLIONE - BLACK</span>
          <div class="price">
            <span class="last-price">29,99 €</span>
            <!-- <span class="full-price">29,99 €</span> -->
          </div>
        </div>
      </div>
      <!-- fine CARD STRIPE-->
    </div>

  </main>
  
</template>

<style lang="scss" scoped>

main {
  margin-top: 60px;
}

/* MAIN */

main .container.flex {
  padding: 40px 0;
  justify-content: start;
  flex-wrap: wrap;
}


.product {
  max-width: 400px;
  width: 33%;
  min-width: 250px;
  padding: 5px;
}

.product img {
  width: 100%;
}

main .image:hover .secondary-image {
  display: block;
}

.product .secondary-image {
  position: absolute;
  top: 0;
  left: 0;
  display: none;
}

.product .image .heart {
  cursor: pointer;
  position: absolute;
  right: 0;
  top: 10px;
  background-color: white;
  padding: 10px;
}

.product .tag {
  position: absolute;
  left: 0;
  bottom: 40px;
  font-size: 0.7rem;
  color: white;
}

.product .image .discount {
  background-color: red;
  padding: 5px 10px;
}

.product .image .sostenibilita {
  background-color: green;
  padding: 5px 10px;
}

.marca,
.modello {
  display: block;
}

.modello {
  font-weight: bold;
}

.price {
  font-size: 0.8rem;
}

.last-price {
  color: red;
  font-weight: bold;
}

.full-price {
  text-decoration: line-through;
}

.heart:hover {
  color: red;
}


</style>