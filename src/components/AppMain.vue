<script>
import products from "../products.js";
import ProductItem from "./ProductItem.vue"
export default {
  name: "AppMain",
  components: {
    ProductItem,
  },
  data() {
    return {
      products
    }
  }

} 
</script>


<template>
  <main id="site_main">

    <div class="main_top">
      <div class="container">
        <div class="row row-cols-6 g-4">

          <ProductItem :image="product.thumb" :title="product.series" :price="product.price" v-for="product in products">
          </ProductItem>

        </div>
      </div>
      <div class="container text-center pb-3 pt-5">
        <button class="btn text-white rounded-0 fs-5 bg_primary">
          LOAD MORE
        </button>
      </div>

    </div>

    <div class="main_store">
      <div class="container">
        <div class="row gap-1 text-center">

          <div class="col">
            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
            <a href="#">DIGITAL COMICS</a>
          </div>
          <div class="col">
            <img src="../assets/img/buy-comics-merchandise.png" alt="">
            <a href="#">DC MERCHANDISE</a>
          </div>
          <div class="col">
            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
            <a href="#">SUBSCRIPTION</a>
          </div>
          <div class="col">
            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
            <a href="#">COMIC SHOP LOCATOR</a>
          </div>
          <div class="col">
            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
            <a href="#">DC POWER VISA</a>
          </div>


        </div>
      </div>
    </div>

  </main>
</template>


<style lang="scss" scoped>
@use '../assets/scss/Partials/variables' as *;

.main_top {
  background-color: $dc_secondary;
  color: white;
  align-items: center;
}

.bg_primary {
  background-color: $dc_primary;
}

.main_store {
  background-color: $dc_primary;
  height: 200px;
  display: flex;
  align-items: center;

  & img {
    width: 50px;
    height: 60px;
  }

  & a {
    color: $dc_white;
    text-decoration: none;
    padding-left: 10px;
    font-size: 13px;
  }
}
</style>