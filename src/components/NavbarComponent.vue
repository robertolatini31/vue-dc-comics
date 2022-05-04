<template>
    <nav>
        <ul>
            <li v-for="item in menu" :key="item.id" :class="item.text === 'comics' ? 'active' : ''"><a :href="item.src" :class="item.text === 'comics' ? 'active-color' : ''">{{item.text}}</a></li>
            
        </ul>
    </nav>
    <!-- ./ navbar  -->
</template>

<script>
export default {
    name: 'NavbarHeader',
    data() {
        return {
            menu: [
                {
                    id: 1,
                    src: '#',
                    text: 'characters'
                },
                {
                    id: 2,
                    src: '#',
                    text: 'comics'
                },
                {
                    id: 3,
                    src: '#',
                    text: 'movies'
                },
                {
                    id: 4,
                    src: '#',
                    text: 'tv'
                },
                {
                    id: 5,
                    src: '#',
                    text: 'games'
                },
                {
                    id: 6,
                    src: '#',
                    text: 'collectibles'
                },
                {
                    id: 7,
                    src: '#',
                    text: 'videos'
                },
                {
                    id: 8,
                    src: '#',
                    text: 'fans'
                },
                {
                   id: 9,
                    src: '#',
                    text: 'news'
                },
                {
                   id: 10,
                    src: '#',
                    text: 'shop'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
nav {
    ul {
        list-style: none;
        li {
            a{
                text-decoration: none;
                color: #464646;
                text-transform: uppercase;
                font-size: 0.8rem;
                font-weight: 600;
            }
            padding: 3rem 0;
            margin: 0 1rem;
            display: inline-block;
            border-bottom: 4px solid transparent;
            &:hover{
                border-color: #0282F9;
            }
            &:hover a {
                color: #0282F9;
            }
        }
    }
}

.active {
    border-bottom: 4px solid #0282F9;
}

.active-color {
    color: #0282F9;
}


</style>