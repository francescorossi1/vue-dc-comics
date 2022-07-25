<template>
  <article class="py-4">
        <div class="container d-flex">
          <figure>
            <img src="../assets/img/buy-comics-digital-comics.png" alt="digital comics">
            <span class="px-2">DIGITAL COMICS</span>
          </figure>
          <figure>
            <img src="../assets/img/buy-comics-merchandise.png" alt="merchandise">
            <span class="px-2">MERCHANDISE</span>
          </figure>
          <figure>
            <img src="../assets/img/buy-comics-subscriptions.png" alt="subscriptions">
            <span class="px-2">SUBSCRIPTIONS</span>
          </figure>
          <figure>
            <img src="../assets/img/buy-comics-shop-locator.png" alt="shop locator">
            <span class="px-2">SHOP LOCATOR</span>
          </figure>
          <figure>
            <img src="../assets/img/buy-dc-power-visa.svg" alt="dc power visa">
            <span class="px-2">DC POWER VISA</span>
          </figure>
        </div>
      </article>
</template>

<script>
export default {
    name: 'FooterArticle'
}
</script>

<style scoped>
article {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  background-color: #0282F9;
}

article figure {
  color: #fff;
  display: flex;
  align-items: center;
  flex-basis: 20%;
}
article img{
  max-width: 50px;
  max-height: 50px;
}
</style>