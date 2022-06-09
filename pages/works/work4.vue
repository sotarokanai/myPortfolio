<template>
    <div class="works">
        <div class="content-area">
            <ttlTxt>霊障 - Book cover</ttlTxt>
            <paragraph>design<br><a href="https://booth.pm/ja/items/2976087">store</a></paragraph>
            <contentImage
            :src="require(`~/assets/img/other/reisho_l.jpg`)"
            default_size="400px"
            ></contentImage>
            <ttlTxt>tool</ttlTxt>
            <paragraph>Blender</paragraph>
        </div>
    </div>
</template>

<style lang="scss">
.works {
    width: 100%;
    overflow: hidden;
    .content-area {
        padding-top: 38px;
        width: 1144px;
        margin: 0 auto;
        iframe {
            width: 100%;
            height: 400px;
            margin-bottom: 34px;
        }
    }
}

@include mobile {
    .works {
        .content-area {
            width: v(680);
            padding-top: v(38);
            iframe {
            width: v(680);
            margin-bottom: v(34);
            }
        }
    }
}
</style>