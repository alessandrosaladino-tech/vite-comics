

<script>

export default {
    name : "AppHeader"
}
</script>

<template>
 
 <header id="site_header">

<div class="container h-100">

  <div class="row align-items-center align-content-center h-100">

    <div class="col-5">
      <img src="../assets/img/dc-logo.png" alt="">
    </div>

    <div class="col-7">
      <nav class="navbar navbar-expand">
        <div class="nav navbar-nav font_size_header nav_container">
          <a class="nav-item nav-link d-flex align-items-center" href="#"><strong>CHARACTERS </strong></a>
          <a class="nav-item nav-link d-flex align-items-center" href="#"><strong>COMICS</strong></a>
          <a class="nav-item nav-link d-flex align-items-center" href="#"><strong>MOVIES</strong></a>
          <a class="nav-item nav-link d-flex align-items-center" href="#"><strong>TV</strong></a>
          <a class="nav-item nav-link d-flex align-items-center" href="#"><strong>GAMES</strong></a>
          <a class="nav-item nav-link d-flex align-items-center" href="#"><strong>COLLECTIBLES</strong></a>
          <a class="nav-item nav-link d-flex align-items-center" href="#"><strong>VIDEOS</strong></a>
          <a class="nav-item nav-link d-flex align-items-center" href="#"><strong>FANS</strong></a>
          <a class="nav-item nav-link d-flex align-items-center" href="#"><strong>NEWS</strong></a>
          <a class="nav-item nav-link d-flex align-items-center" href="#"><strong>SHOP</strong></a>
        </div>

      </nav>
    </div>
  </div>
</div>

</header>

</template>

<style lang="scss" scoped>

@use '../assets/scss/Partials/variables' as *;

#site_header {
    height: 150px;
}

.font_size_header {
    font-size: 15px;

    & a:hover {
        border-bottom: 3px solid $dc_primary;
    }

    & a {
        height: 100%;
    }
}

.nav_container {
    height: 150px;
}
</style>
