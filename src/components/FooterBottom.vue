<template>
    <div class="footer-bottom">
        <nav>
            <div class="navbar">
                <div class="container d-flex justify-content-between align-items-center h-100">
                    <div>
                        <a href="#" class="blue-border-btn">SIGN-UP NOW!</a>
                    </div>
                    <div class="d-flex">
                        <a href="#" class="px-2 blue-text">FOLLOW US</a>
                        <ul class="d-flex flex-grow">
                            <li v-for="social in socials" :key="social.id"><a href="#"><img :src="social.src"
                                        :alt="social.name"></a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </nav>
    </div>
</template>

<script>
export default {
    name: 'FooterBottom',
    data() {
        return {
            socials: [
                { id: 1, name: 'facebook', src: require('../assets/img/footer-facebook.png'), url: '#' },
                { id: 2, name: 'twitter', src: require('../assets/img/footer-twitter.png'), url: '#' },
                { id: 3, name: 'youtube', src: require('../assets/img/footer-youtube.png'), url: '#' },
                { id: 4, name: 'pinterest', src: require('../assets/img/footer-pinterest.png'), url: '#' },
                { id: 5, name: 'periscope', src: require('../assets/img/footer-periscope.png'), url: '#' }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.footer-bottom {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    background-color: #303030;
    line-height: 100%;

    ul li {
        padding: 0 10px;

        img {
            vertical-align: middle;
        }
    }
}

.blue-border-btn {
    color: #fff;
    padding: 10px;
    border: 2px solid #0282F9;
}
</style>