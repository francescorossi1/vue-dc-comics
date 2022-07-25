<template>
  <header>
      <div class="navbar">
        <div class="container d-flex justify-content-between align-items-center h-100">
          <figure class="h-100 p-2">
            <img src="../assets/img/dc-logo.png" alt="dc logo">
          </figure>
          <div>
            <ul class="d-flex flex-grow">
              <li><a href="#">CHARACTERS</a></li>
              <li class="active"><a href="#">COMICS</a></li>
              <li><a href="#">MOVIES</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">GAMES</a></li>
              <li><a href="#">COLLECTIBLES</a></li>
              <li><a href="#">VIDEOS</a></li>
              <li><a href="#">FANS</a></li>
              <li><a href="#">NEWS</a></li>
              <li><a href="#">SHOP</a></li>
            </ul>
          </div>
        </div>
      </div>
    </header>
</template>

<script>
export default {
    name: 'MainHeader'
}
</script>

<style>
.navbar ul li {
  padding: 0 15px;
}

.active {
  border-bottom: 5px solid #0282F9;
}

.active a {
  color: #0282F9;
}
</style>