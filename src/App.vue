<template>
  <div>
    <MainHeader />
    <MainContent />
    <MainFooter />
  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue'
import MainContent from './components/MainContent.vue'
import MainFooter from './components/MainFooter.vue'

export default {
  name: 'App',
  components: {
    MainHeader,
    MainContent,
    MainFooter
}
}
</script>

<style>
/* Generics */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: "Segoe UI", "Open Sans", Helvetica, sans-serif;
}

img {
  max-height: 100%;
}

.container {
  max-width: 80%;
  margin: 0 auto;
}

ul {
  list-style-type: none;
  padding: 0;
}

a {
  text-decoration: none;
  color: #303030;
}

/* Navbar */
.navbar {
  height: 100px;
  line-height: 100px;
  font-weight: bold;
}

.navbar ul li {
  padding: 0 15px;
}

/* Utils */
.p-0 {
  padding: 0;
}

.p-1 {
  padding: 5px;
}

.p-2 {
  padding: 10px;
}

.p-3 {
  padding: 20px;
}

.p-4 {
  padding: 35px;
}

.p-5 {
  padding: 50px;
}

.py-1 {
  padding: 5px 0;
}

.py-2 {
  padding: 10px 0;
}

.py-3 {
  padding: 20px 0;
}

.py-4 {
  padding: 35px 0;
}

.py-5 {
  padding: 50px 0;
}

.px-1 {
  padding: 0 5px;
}

.px-2 {
  padding: 0 10px;
}

.px-3 {
  padding: 0 20px;
}

.px-4 {
  padding: 0 35px;
}

.px-5 {
  padding: 0 50px;
}

.h-100 {
  height: 100%;
}

.blue-text {
  color: #0282F9;
}

.d-flex {
  display: flex;
}

.justify-content-between {
  justify-content: space-between;
}

.align-items-center {
  align-items: center;
}

.text-center {
  text-align: center;
}
</style>
