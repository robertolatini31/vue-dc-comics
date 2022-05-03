<template>
    <nav>
        <ul>
            <li v-for="(li, index) in menu" :key="index">{{li.li}}</li>
            
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
                    li: 'characters'
                },
                {
                    li: 'comics'
                },
                {
                    li: 'movies'
                },
                {
                    li: 'tv'
                },
                {
                    li: 'games'
                },
                {
                    li: 'collectibles'
                },
                {
                    li: 'videos'
                },
                {
                    li: 'fans'
                },
                {
                    li: 'news'
                },
                {
                    li: 'shop'
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
            color: #464646;
            text-transform: uppercase;
            display: inline-block;
            padding: 2rem 1rem;
            font-size: 0.8rem;
            font-weight: 600;
            cursor: pointer;
        }
    }
}

.active {
    color: #0282F9;
    position: relative;
}

.active:before {
  content: "";
  position: absolute;
  left: 50%;
  bottom: 0;
  transform: translate(-50%,-50%);
  height: 1px;
  width: 50%; 
  border-bottom: 2px solid #0282F9;
}
</style>