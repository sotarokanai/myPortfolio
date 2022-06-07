<template>
    <div class="large-txt">
        <p :style="{color: fore_color}"><slot>犬が犬であるために</slot></p>
    </div>
</template>

<script>
export default {
    props: {
        fore_color: {
            type: String,
            default:"#00000"
        }
    }   
}
</script>

<style lang="scss">
    .large-txt {
        margin-bottom: 24px;
        p {
            border-left: solid 1px $black;
            font-size: 24px;
            padding-left: 24px;
        }
    }

    @include mobile {
        .large-txt {
            margin-bottom: v(24);
            p {
                border-left: solid 0.3vw $black;
                font-size: v(36);
                padding-left: 3vw;
            }
        }
    }
</style>