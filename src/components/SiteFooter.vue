<template>
    <footer>
        <div class="container">
            <div class="row">
                <div class="col-6">
                <button>sing-up now!</button>
            </div>
            <div class="col-6 text-right">
                <h3>follow us</h3>
                <img src="@/assets/img/footer-facebook.png" alt="">
                <img src="@/assets/img/footer-twitter.png" alt="">
                <img src="@/assets/img/footer-youtube.png" alt="">
                <img src="@/assets/img/footer-pinterest.png" alt="">
                <img src="@/assets/img/footer-periscope.png" alt="">
            </div>
            </div>
            <!-- /.row -->
        </div>
        <!-- /.container -->
    </footer>
</template>

<script>
export default {
    name: 'SiteFooter',
}
</script>

<style lang="scss" scoped>

footer {
    padding: 2rem 1rem;
    background-color: rgb(69, 69, 69);
}

h3 {
    text-transform: uppercase;
    font-weight: 900;
    color: blue;
}

button {
    text-transform: uppercase;
    background-color: transparent;
    padding: 0.7rem;
    border: 2px solid blue;
    color: white;
    font-weight: 600;
}

.text-right {
   display: flex;
    justify-content: end;
    align-items: center;
    column-gap: 1rem;
}
</style>