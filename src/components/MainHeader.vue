<template>
  <header>
    <div class="navbar">
      <div class="container d-flex justify-content-between align-items-center h-100">
        <figure class="h-100 p-2">
          <img src="../assets/img/dc-logo.png" alt="dc logo">
        </figure>
        <div>
          <ul class="d-flex flex-grow">
            <li :class="{ 'active': link.active }" v-for="link in headerLinks" :key="link.id"><a href="#">{{ link.name
            }}</a></li>
          </ul>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'MainHeader',
  data() {
    return {
      headerLinks: [
        { id: 1, url: '#', name: 'CHARACTERS', active: false },
        { id: 2, url: '#', name: 'COMICS', active: true },
        { id: 3, url: '#', name: 'MOVIES', active: false },
        { id: 4, url: '#', name: 'TV', active: false },
        { id: 5, url: '#', name: 'GAMES', active: false },
        { id: 6, url: '#', name: 'COLLECTIBLES', active: false },
        { id: 7, url: '#', name: 'VIDEOS', active: false },
        { id: 8, url: '#', name: 'FANS', active: false },
        { id: 9, url: '#', name: 'NEWS', active: false },
        { id: 10, url: '#', name: 'SHOP', active: false }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.active {
  border-bottom: 5px solid #0282F9;

  a {
    color: #0282F9;
  }
}
</style>