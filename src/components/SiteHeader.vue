<template>
   <header>
        <div class="container">
        <div class="row">
            <div class="col-4">
                <img src="@/assets/img/dc-logo.png" alt="">
            </div>
            <!--/.logo_header  -->
            <div class="col-8">
                <NavbarComponent />
            </div>
            <!--/.navbar_header  -->
        </div>
        <!-- /.row -->
    </div>
    <!-- /.container -->
   </header>
   <!-- /.SiteHeader -->
</template>

<script>
import NavbarComponent from './NavbarComponent.vue'
export default {
   name: 'SiteHeader',
   components: {
       NavbarComponent,
   }
}
</script>


<style lang="scss" scoped>
header {
    img {
        max-width: 70px;
    }
    padding: 0 1rem;
    .col-4, .col-8 {
        display: flex;
        align-items: center;
        justify-content: flex-start;
    }
}
</style>