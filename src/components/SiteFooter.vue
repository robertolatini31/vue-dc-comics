<template>
    <footer>
        <div class="container">
            <div class="row">
                <div class="col-6">
                <button>sing-up now!</button>
            </div>
            <div class="col-6 social-col">
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

.col-6 {
    margin-bottom: 2rem;
    flex-grow: 1;
}

footer {
    padding: 2rem 1rem 0 1rem;
    background-color: $dc-footer-dark;
}

h3 {
    text-transform: uppercase;
    font-weight: 900;
    color: $dc-primary;
}

button {
    text-transform: uppercase;
    background-color: transparent;
    padding: 0.7rem;
    border: 2px solid $dc-primary;
    color: white;
    font-weight: 600;
}

.social-col {
    display: flex;
    justify-content: flex-end;
    align-items: center;
    column-gap: 1rem;
    row-gap: 1rem;
    flex-wrap: wrap;
}
</style>