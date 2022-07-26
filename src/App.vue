<template>
  <div>
    <MainHeader />
    <MainContent :comics-list="ComicsList"/>
    <MainFooter />
  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue'
import MainContent from './components/MainContent.vue'
import MainFooter from './components/MainFooter.vue'
import ComicsJson from './dc-comics.json'

export default {
  name: 'App',
  components: {
    MainHeader,
    MainContent,
    MainFooter,
},data(){
  return {
    ComicsList: ComicsJson
  }
}
}
</script>

<style lang="scss">
@import './assets/sass/style';


.navbar {
  height: 100px;
  line-height: 100px;
  font-weight: bold;


  ul li{
    padding: 0 15px;
  }
}

</style>
