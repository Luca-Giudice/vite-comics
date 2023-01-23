<script>
export default {
    name: 'appFooter'
}
</script>

<template>
    <footer>
        <section class="container">
            <nav class="nav-footer">
                <div>
                    <div class="footer-col">
                        <h4>DC COMICS</h4>
                        <ul>
                            <li>
                                <a href="#">Charters</a>
                            </li>
                            <li>
                                <a href="#">Comics</a>
                            </li>
                            <li>
                                <a href="#">Movies</a>
                            </li>
                            <li>
                                <a href="#">TV</a>
                            </li>
                            <li>
                                <a href="#">Games</a>
                            </li>
                            <li>
                                <a href="#">Videos</a>
                            </li>
                            <li>
                                <a href="#">News</a>
                            </li>
                        </ul>
                    
                    </div>
                    <div class="footer-col">
                        <h4>SHOP</h4>
                        <ul>
                            <li>
                                <a href="#">Shop DC</a>
                            </li>
                            <li>
                                <a href="#">Shop DC Collectibles</a>
                            </li>

                        </ul>
                    </div>
                </div>
                
                <div class="footer-col">
                    <h4>DC</h4>
                    <ul>
                        <li>
                            <a href="#">Terms Of Use</a>
                        </li>
                        <li>
                            <a href="#">Privacy policy (New)</a>
                        </li>
                        <li>
                            <a href="#">Ad Choices</a>
                        </li>
                        <li>
                            <a href="#">Advertising</a>
                        </li>
                        <li>
                            <a href="#">Jobs</a>
                        </li>
                        <li>
                            <a href="#">Subscriptions</a>
                        </li>
                        <li>
                            <a href="#">Talent Workshops</a>
                        </li>
                        <li>
                            <a href="#">CPSC Certificates</a>
                        </li>
                        <li>
                            <a href="#">Ratings</a>
                        </li>
                        <li>
                            <a href="#">Shop Help</a>
                        </li>
                        <li>
                            <a href="#">Contact Us</a>
                        </li>
                    </ul>

                </div>
                <div class="footer-col">
                    <h4>SITES</h4>
                    <ul>
                        <li>
                            <a href="#">DC</a>
                        </li>
                        <li>
                            <a href="#">MAD Magazine</a>
                        </li>
                        <li>
                            <a href="#">DC Kids</a>
                        </li>
                        <li>
                            <a href="#">DC Universe</a>
                        </li>
                        <li>
                            <a href="#">DC Power Visa</a>
                        </li>
                    </ul>
                
                </div>
            </nav>

        </section>
        <section class="social">
            <section class="container">
                <button> SING-UP NOW!</button>

            </section>

        </section>
    </footer>

</template>

<style scoped>
footer{
    background-image: url(../assets/img/footer-bg.jpg);
    color: white;
    padding-top: 15px;
}

.nav-footer{
    display: flex;
    gap: 30px;
}

li{
    list-style-type: none;
}

a{
    color: gray;
    font-size: 12px;
}

.social{
    background-color: rgb(48, 48, 48);
}
</style>