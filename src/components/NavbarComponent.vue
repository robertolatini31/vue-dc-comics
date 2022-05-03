<template>
    <nav>
        <ul>
            <li>characters</li>
            <li class="active">comics</li>
            <li>movies</li>
            <li>tv</li>
            <li>games</li>
            <li>collectibles</li>
            <li>videos</li>
            <li>fans</li>
            <li>news</li>
            <li>shop</li>
        </ul>
    </nav>
    <!-- ./ navbar  -->
</template>

<script>
export default {
    name: 'NavbarHeader'
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