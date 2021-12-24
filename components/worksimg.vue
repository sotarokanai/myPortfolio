<template>
    <a @click="$router.push(linkPath)">
        <img :src="src" alt="">
        <p>{{worksTtl}}</p>
    </a>
</template>

<script>
export default {
    props: {
        src: {
            default: require('~/assets/img/1.png'),
            type: String,
        },
        worksTtl: {
            default: 'サンプル',
            type: String,
        },
        linkPath: {
            default: '/works',
            type: String,
        }
    }
}
</script>

<style lang="scss">
a {
    margin: 0.1vw;
    position: relative;
    img {
        width: 28vw;  
    }
    p {
        margin: -14.3vw;
        color: #fff;
        display: none;
        font-size: 16px;
    }
}
a:hover {
    filter: brightness(1.4);
    p {
        display: block;
    }
}
</style>