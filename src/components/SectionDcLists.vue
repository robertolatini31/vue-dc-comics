<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="col-6 col-lists">
                    <div class="row">
                        <div class="col-4" v-for="({title, links}, index) in menuArray" :key="index">
                            <h3>{{title}}</h3>
                            <ul>
                                <li v-for="({href, text}, index) in links" :key="index"><a :href="href">{{text}}</a></li>
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
    data() {
        return {
            menuArray: [
                {
                    title: 'dc comics',
                    links: [
                        {
                            href: '#',
                            text: 'Characters'
                        },
                        {
                            href: '#',
                            text: 'Comics'
                        },
                        {
                            href: '#',
                            text: 'Movies'
                        },
                        {
                            href: '#',
                            text: 'TV'
                        },
                        {
                            href: '#',
                            text: 'Games'
                        },
                        {
                            href: '#',
                            text: 'Videos'
                        },
                        {
                            href: '#',
                            text: 'News'
                        },
                    ]
                },
                {
                    title: 'dc',
                    links: [
                        {
                            href: '#',
                            text: 'Terms Of Use'
                        },
                        {
                            href: '#',
                            text: 'Privacy policy (New)'
                        },
                        {
                            href: '#',
                            text: 'ad Choices'
                        },
                        {
                            href: '#',
                            text: 'Advertising'
                        },
                        {
                            href: '#',
                            text: 'Jobs'
                        },
                        {
                            href: '#',
                            text: 'Subscriptions'
                        },
                        {
                            href: '#',
                            text: 'Talent Workshops'
                        },
                        {
                            href: '#',
                            text: 'CPSC Certificates'
                        },
                        {
                            href: '#',
                            text: 'Ratings'
                        },
                        {
                            href: '#',
                            text: 'Shop Help'
                        },
                        {
                            href: '#',
                            text: 'Contact Us'
                        },
                    ]
                },
                {
                    title: 'sites',
                    links: [
                        {
                            href: '#',
                            text: 'DC'
                        },
                        {
                            href: '#',
                            text: 'MAD Magazine'
                        },
                        {
                            href: '#',
                            text: 'DC Kids'
                        },
                        {
                            href: '#',
                            text: 'DC Universe'
                        },
                        {
                            href: '#',
                            text: 'DC Power Visa'
                        },
                    ],
                },
                {
                    title: 'shop',
                    links: [
                        {
                            href: '#',
                            text: 'Shop DC'
                        },
                        {
                            href: '#',
                            text: 'Shop DC Collectibles'
                        }
                    ]
                }
            ]
        }
    }
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
            color: $dc-list-text;
            font-weight: 500;
        }
    }
    
}

.col-4 {
    min-width: 135px;
}

.col-lists {
    padding: 3rem 1rem;
}


h3 {
        color: white;
        text-transform: uppercase;
        margin: 1rem 0;
}

section {
    background-image: url('@/assets/img/footer-bg.jpg');
    background-size: cover;
}

.bg-logo-big {
    background-image: url('@/assets/img/dc-logo-bg.png');
    background-size: cover;
    background-position: center;
}

</style>