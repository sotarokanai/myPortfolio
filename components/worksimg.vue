<template>   
    <a class="work-link" @click="$router.push(linkPath)">
        <img :src="src" alt="">
        <p>{{worksTtl}}</p>
    </a>
</template>

<script>
export default {
    props: {
        src: {
            default: require('~/assets/img/works/1.jpg'),
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
.work-link {
    margin-bottom: 34px;
    text-decoration: none;
    img {
        width: 368px;
        margin-bottom: 8px;
    }
    p {
        font-size: 14px;
    }
}
a:hover {
    filter: brightness(0.8);
    p {
        display: block;
    }
}

@include mobile {
    .work-link {
        margin-bottom: v(35);
        img {
            width: v(680);
            margin-bottom: v(12);
        }
        p {
            font-size: v(20);
        }
    }
}
</style>