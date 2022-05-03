<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="col-6 py-3">
                    <div class="row">
                        <div class="col-4">
                            <h3>dc comics</h3>
                            <ul>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Comics</a></li>
                                <li><a href="#">Movies</a></li>
                                <li><a href="#">TV</a></li>
                                <li><a href="#">Games</a></li>
                                <li><a href="#">Videos</a></li>
                                <li><a href="#">News</a></li>
                            </ul>
                            <h3>shop</h3>
                            <ul>
                                <li><a href="#">Shop DC</a></li>
                                <li><a href="#">Shop DC Collectibles</a></li>
                            </ul>
                        </div>
                        <div class="col-4">
                            <h3>dc</h3>
                            <ul>
                                <li><a href="#">Terms Of Use</a></li>
                                <li><a href="#">Privacy policy (New)</a></li>
                                <li><a href="#">ad Choices</a></li>
                                <li><a href="#">Advertising</a></li>
                                <li><a href="#">Jobs</a></li>
                                <li><a href="#">Subscriptions</a></li>
                                <li><a href="#">Talent Workshops</a></li>
                                <li><a href="#">CPSC Certificates</a></li>
                                <li><a href="#">Ratings</a></li>
                                <li><a href="#">Shop Help</a></li>
                                <li><a href="#">Contact Us</a></li>
                            </ul>
                        </div>
                        <div class="col-4">
                            <h3>sites</h3>
                            <ul>
                                <li><a href="#">DC</a></li>
                                <li><a href="#">MAD Magazine</a></li>
                                <li><a href="#">DC Kids</a></li>
                                <li><a href="#">DC Universe</a></li>
                                <li><a href="#">DC Power Visa</a></li>
                            </ul>
                        </div>
                    </div>
                    <!-- /.row -->
                </div>
                <!-- /.col-6 -->
                <div class="col-6 bg-logo-big"></div>
                <!-- /.col-6 -->
            </div>
            <!-- /.row -->
        </div>
        <!-- /.container -->
    </section>
</template>

<script>
export default {
    name: 'SectionDcLists',
}
</script>

<style lang="scss" scoped>
ul {
    list-style: none;
    line-height: 1.2rem;
    li {  
        font-size: 0.8rem;
        a {
            text-decoration: none;
            color: #959595;
        }
    }
    
}

.py-3 {
    padding: 3rem 0;
}

h3 {
        color: white;
        text-transform: uppercase;
        margin: 1rem 0;
}

section {
    background-image: url('@/assets/img/footer-bg.jpg');
    background-size: cover;
    padding: 0 1rem;
}

.bg-logo-big {
    background-image: url('@/assets/img/dc-logo-bg.png');
    background-size: cover;
    background-position: center;
}

</style>