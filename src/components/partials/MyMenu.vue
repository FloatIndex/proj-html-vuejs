<template>
    <ul>
        <li v-for="(item, index) in menu" :key="index"><a href="#">{{item}}</a></li>
        <!-- <li><a href="#">home</a></li>
        <li><a href="#">about</a></li>
        <li><a href="#">projects</a></li>
        <li><a href="#">services</a></li>
        <li><a href="#">blog</a></li>
        <li><a href="#">contact</a></li> -->
    </ul>
</template>

<script>
export default {
    name: 'MenuList',
    props: {
        menu: Array
    }
}
</script>

<style lang="scss" scoped>
ul {
    list-style: none;

    li {
        display: inline-block;
        margin-left: 30px;

        a {
            text-transform: uppercase;
        }
    }
}
</style>