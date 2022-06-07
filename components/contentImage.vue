<template>
    <div class="content-image">
        <img :style="{width: default_size}" :src="src" alt="">
    </div>  
</template>

<script>
export default {
    props: {
        src: {
            default: require('~/assets/img/1.jpg'),
            type: String,
        },
        default_size: {
            type: String,
            default:"100%"
        }
    }
}
</script>

<style lang="scss">
.content-image {
    margin-bottom: 34px;
    text-align: center;

    img {
        width: 100%;
    }
}

@include mobile {
    .content-image {
        margin-bottom: 5vw;
        img {
            width: 90vw!important;
        }
    }
}

</style>