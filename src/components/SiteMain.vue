<template>
    <main>
        <JumbotronComponent />
        <div class="container">
            <h3 class="current_series">current series</h3>
            <!-- /.current_series -->
            
            
        </div>
        <!-- /.container -->
    </main>
</template>

<script>
import JumbotronComponent from '@/components/JumbotronComponent.vue'
export default {
    name: 'SiteMain',
    components: {
        JumbotronComponent,
    }
}
</script>

<style lang="scss" scoped>
.container {
    position: relative;
    h3 {
    position: absolute;
    top: -26px;
    left: 16px;
    text-transform: uppercase;
    background-color: #0282F9;
    padding: 0.5rem 1rem;
    }
}

main {
    background-color: black;
    color: white;
    height: 500px;
}
 
</style>