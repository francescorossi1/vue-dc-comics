<template>
  <main>
    <div class="jumbotron">
      <div class="main-content py-3">
        <div class="container">
          <a href="#" class="blue-button font-20 moved">CURRENT SERIES</a>
          <div class="d-flex flex-wrap justify-content-center py-3">
            <figure v-for="(comic, i) in comicsList" :key="i">
                <img :src="comic.thumb" :alt="comic.series">
              <figcaption>{{ comic.series }}</figcaption>
            </figure>
          </div>
          <div class="d-flex justify-content-center">
            <a href="#" class="blue-button large">LOAD MORE</a>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: 'MainContent',
  props: { comicsList: Array }
}
</script>

<style lang="scss" scoped>
.jumbotron {
  margin-top: 2.5px;
  background-image: url('../assets/img/jumbotron.jpg');
  background-position: top center;
  padding-top: 400px;

  .main-content {
    font-size: 14px;
    background-color: #1C1C1C;
    color: #fff;

    figure {
      flex-basis: calc(100% / 6 - 20px);
      padding: 10px;
      margin-bottom: 30px;
      height: calc(80vw / 6 - 20px);

        img {
          height: 140px;
          width: 140px;
          object-fit: cover;
          object-position: top;
          overflow: hidden;
        }
      }
    }
  }

.blue-button{
  font-weight: bold;
  background-color: #0282F9;
  color: white;
  padding: 5px 15px;

  &.moved{
    position: relative;
    left: 30px;
    bottom: 30px;
  }

  &.large{
    padding-left: 30px;
    padding-right: 30px;
  }
}
</style>