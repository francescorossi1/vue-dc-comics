<template>
  <footer>
    <FooterArticle />
    <FooterTop />
    <FooterBottom />
  </footer>
</template>

<script>
import FooterArticle from './FooterArticle.vue'
import FooterTop from './FooterTop.vue'
import FooterBottom from './FooterBottom.vue'
export default {
    name: 'MainFooter',
    components: {
    FooterArticle,
    FooterTop,
    FooterBottom
}
}
</script>

<style lang="scss" scoped>
footer {
  height: calc(100vh - 250px);
  position: relative;
}
</style>