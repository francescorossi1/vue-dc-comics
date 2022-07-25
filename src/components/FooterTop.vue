<template>
    <div class="footer-top h-100">
        <div class="container d-flex justify-content-between h-100">
          <div class="footer-links d-flex h-100">
            <div v-for="section in sections" :key="section.id" class="px-2">
              <h3 class="py-1">{{section.name}}</h3>
              <ul>
                <li v-for="link in section.links" :key="link.id"><a href="#">{{link}}</a></li>
              </ul>
            </div>
          </div>
          <div class="footer-img h-100">
              <img src="../assets/img/dc-logo-bg.png" alt="dc logo">
          </div>
        </div>
      </div>
</template>

<script>
    export default {
        name: 'FooterTop',
        data(){
            return {
                sections: [
                    {id: 1, name: 'DC COMICS', links: ['Characters','Comics','Movies','TV','Games','Videos','News']},
                    {id: 2, name: 'SHOP', links: ['Shop DC','Shop DC Collectibles']},
                    {id: 3, name: 'DC', links: ['Terms of use','Privacy Policy (new)','Ad Choices','Advertising','Jobs','Subscriptions','Talent Workshop','CPSC Certificates','Ratings','Shop Help','Contact Us']},
                    {id: 4, name: 'SITES', links: ['DC','MAD Magazine','DC Kids','DC Universe','DC Power Visa']}
                ]
            }
        }
    }
</script>

<style scoped>
.footer-top {
  color: #fff;
  background-image: url(../assets/img/footer-bg.jpg)
}

footer a {
  color: #6D6A68;
}

.footer-links,
.footer-img {
  flex-basis: 30%;
}

.footer-links {
  padding-top: 140px;
}

.footer-links li {
  font-size: 12px;
  line-height: 20px;
}
</style>