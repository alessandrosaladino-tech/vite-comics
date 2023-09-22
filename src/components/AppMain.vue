<script>
export default {
   name:"AppMain"

} 
</script>


<template>
    
    <main id="site_main">

<div class="main_top">
  <div class="container">
    <h2> --> Content goes here &lt;--</h2>
  </div>
</div>

<div class="main_store">
  <div class="container">
     <div class="row gap-1">

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
    height: 150px ;
    display: flex;
    align-items: center;
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