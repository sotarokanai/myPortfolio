<template>
    <div class="article-ttl">
        <p :style="{color: fore_color}"><a @click="$router.push(linkPath)">/<slot>犬が犬であるために</slot></a></p>
    </div>
</template>

<script>
export default {
    props: {
        fore_color: {
            type: String,
            default:"#00000"
        },
        linkPath: {
            default: '/article',
            type: String,
        }
    }   
}
</script>

<style lang="scss">
    .article-ttl {
        margin-bottom: 24px;
        p {
            font-size: 24px;
        }
    }

    @include mobile {
        .article-ttl {
            margin-bottom: v(24);
            p {
                font-size: v(36);
            }
        }
    }
</style>