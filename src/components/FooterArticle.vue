<template>
  <article class="py-4">
    <div class="container d-flex">
      <figure v-for="image in images" :key="image.id">
        <img :src="image.src" :alt="image.name">
        <span class="px-2">{{ image.name.toUpperCase() }}</span>
      </figure>
    </div>
  </article>
</template>

<script>
export default {
  name: 'FooterArticle',
  data() {
    return {
      images: [
        { id: 1, src: require("../assets/img/buy-comics-digital-comics.png"), name: "digital comics" },
        { id: 2, src: require("../assets/img/buy-comics-merchandise.png"), name: "merchandise" },
        { id: 3, src: require("../assets/img/buy-comics-subscriptions.png"), name: "subscriptions" },
        { id: 4, src: require("../assets/img/buy-comics-shop-locator.png"), name: "shop locator" },
        { id: 5, src: require("../assets/img/buy-dc-power-visa.svg"), name: "dc power visa" }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
article {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  background-color: #0282F9;


  figure {
  color: #fff;
  display: flex;
  align-items: center;
  flex-basis: 20%;
  }

  img {
  max-width: 50px;
  max-height: 50px;
  }
}
</style>