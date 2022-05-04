<template>
   <section>
        <div class="container">
        <div class="row">
            <div class="col-2special" v-for="({href, src, text}, index) in services" :key="index">
                <div>
                    <img :src="src" alt="">
                    <a :href="href">{{text}}</a>
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
    data() {
        return {
            services: [
                {
                    href: '#',
                    src: require('@/assets/img/buy-comics-digital-comics.png'),
                    text: 'digital comics'
                },
                {
                    href: '#',
                    src: require('@/assets/img/buy-comics-merchandise.png'),
                    text: 'dc merchandise'
                },
                {
                    href: '#',
                    src: require('@/assets/img/buy-comics-subscriptions.png'),
                    text: 'subscriptions'
                },
                {
                    href: '#',
                    src: require('@/assets/img/buy-comics-shop-locator.png'),
                    text: 'comic shop locator'
                },
                {
                    href: '#',
                    src: require('@/assets/img/buy-dc-power-visa.svg'),
                    text: 'dc power visa'
                },
            ]
        }
    }
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
    background-color: $dc-primary;
    padding: 3rem 1rem;
}

a {
    text-decoration: none;
    color: white;
    text-transform: uppercase;
    font-size: 0.8rem;
    font-weight: 600;
}

img {
    max-width: 60px;
    aspect-ratio: 1.1;
    object-fit: contain;
}

</style>