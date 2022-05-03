<template>
   <section>
        <div class="container">
        <div class="row">
            <div class="col-2special">
                <div>
                    <img src="@/assets/img/buy-comics-digital-comics.png" alt="">
                    <a href="#">digital comics</a>
                </div>
            </div>
            <div class="col-2special">
                <div>
                    <img src="@/assets/img/buy-comics-merchandise.png" alt="">
                    <a href="#">dc merchandise</a>
                </div>
            </div>
            <div class="col-2special">
                <div>
                    <img src="@/assets/img/buy-comics-subscriptions.png" alt="">
                    <a href="#">subscriptions</a>
                </div>
            </div>
            <div class="col-2special">
                <div>
                    <img src="@/assets/img/buy-comics-shop-locator.png" alt="">
                    <a href="#">comic shop locator</a>
                </div>
            </div>
            <div class="col-2special">
                <div>
                    <img src="@/assets/img/buy-dc-power-visa.svg" alt="">
                    <a href="#">dc power visa</a>
                </div>
            </div>
            
        </div>
        <!-- /.row -->
    </div>
    <!-- /.container -->
   </section>
</template>

<script>
export default {
    name: 'ServicesComponent',
}
</script>

<style lang="scss" scoped>

.row {
    align-items: center;
    justify-content: center;
    column-gap: 2rem;
    row-gap: 1rem;
}

.col-2special {
    flex: 1 1 auto;
}

.col-2special>div {
    display: flex;
    align-items: center;
    justify-content: center;    
    column-gap: 0.5rem;
}

section {
    background-color: blue;
    padding: 3rem 1rem;
}

a {
    
    text-decoration: none;
    color: white;
    text-transform: uppercase;
    font-size: 0.7rem;
    font-weight: 500;
}

img {
    max-width: 60px;
    aspect-ratio: 1.1;
    object-fit: contain;
}

</style>