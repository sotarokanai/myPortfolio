<template>
    <div class="works">
        <div class="content-area">
            <ttlTxt>random</ttlTxt>
            <paragraph>TouchDesignerを扱ったランダム表現とAxiDrawによるプリント。</paragraph>
             <contentImage
            :src="require(`~/assets/img/other/pn7.png`)"
            default_size="600px"
            ></contentImage>
             <contentImage
            :src="require(`~/assets/img/other/4.jpg`)"
            ></contentImage>
            <contentImage
            :src="require(`~/assets/img/other/axi.jpg`)"
            ></contentImage>
            <ttlTxt>tool</ttlTxt>
            <paragraph>TouchDesigner, AxiDraw</paragraph>
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