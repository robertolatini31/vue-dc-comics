<template>
    <main>
        <JumbotronComponent />
        <div class="container">
            <h3 class="current_series">current series</h3>
            <!-- /.current_series -->
            <div class="container_cards">
                <div class="row">
                    <div class="col-2" v-for="(book, index) in books" :key="index">
                        <div class="card">
                            <img :src="book.thumb" alt="">
                            <h4>{{book.series}}</h4>
                        </div>
                        <!-- /.card -->
                    </div>
                </div>
            </div>
            <!-- /.container_cards -->

            <div class="btn_container">
                <button>load more</button>
            </div>
            <!-- /.btn_container -->
            
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
    },
    data() {
        return {
            books: [
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    price: "$19.99",
                    series: "Action Comics",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    price: "$3.99",
                    series: "American Vampire 1976",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    price: "$16.99",
                    series: "Aquaman",
                    type: "graphic novel"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    price: "$2.99",
                    series: "Batgirl",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    price: "$3.99",
                    series: "Batman",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    price: "$2.99",
                    series: "Batman Beyond",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    price: "$3.99",
                    series: "Batman/Superman",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    price: "$4.99",
                    series: "Batman/Superman Annual",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    price: "$5.99",
                    series: "Batman: The Joker War Zone",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    price: "$6.99",
                    series: "Batman: Three Jokers",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    price: "$4.99",
                    series: "Batman: White Knight Presents: Harley Quinn",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    price: "$16.99",
                    series: "Catwoman",
                    type: "graphic novel"
                }
            ]
        }
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
    background-color: $dc-primary;
    padding: 0.5rem 1rem;
    }

    .row {
        justify-content: center;
    }

    .col-2 {
            min-width: 240px;
            padding: 3rem 0.5rem;
        .card {
            img {
                width: 220%;
                height: 220px;
                aspect-ratio: 1/1;
                object-fit: cover;
                object-position: top;
            }
            h4 {
                text-transform: uppercase;
                padding: 0.5rem 0;
                font-weight: 500;
                font-size: 1rem;
            }
        }
        
    }
    .btn_container {
        display: flex;
        justify-content: center;
        padding: 2rem;
        button {
            padding: 0.5rem 3rem;
            font-weight: 600;
            text-transform: uppercase;
            color: white;
            background-color: $dc-primary;
            border: none;
        }
    
    }
}
main {
    background-color: $dc-main-dark;
    color: white;
}
 
</style>