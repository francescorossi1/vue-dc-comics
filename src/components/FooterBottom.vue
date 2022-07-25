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
                            <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="facebook"></a></li>
                            <li><a href="#"><img src="../assets/img/footer-twitter.png" alt="twitter"></a></li>
                            <li><a href="#"><img src="../assets/img/footer-youtube.png" alt="youtube"></a></li>
                            <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a></li>
                            <li><a href="#"><img src="../assets/img/footer-periscope.png" alt="periscope"></a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </nav>
    </div>
</template>

<script>
export default {
    name: 'FooterBottom'
}
</script>

<style>
.footer-bottom {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    background-color: #303030;
    line-height: 100%;
}

.footer-bottom ul li {
    padding: 0 10px;
}

.footer-bottom li img {
    vertical-align: middle;
}

.blue-border-btn {
    color: #fff;
    padding: 10px;
    border: 2px solid #0282F9;
}
</style>