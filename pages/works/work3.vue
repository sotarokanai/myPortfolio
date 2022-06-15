<template>
    <div class="works">
        <div class="content-area">
            <ttlTxt>DANCE</ttlTxt>
            <paragraph>1本の線がリズムに合わせ跳ねるように動く。赤い線の軌跡を青、緑の線が後を追うように続く。<br>※動画では都合上音声を消してあります。</paragraph>
            <contentImage
                :src="require(`~/assets/img/works/3.jpg`)"
            ></contentImage>
            <iframe src="https://www.youtube.com/embed/1sW_sl2yVH8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            <ttlTxt>tool</ttlTxt>
            <paragraph>TouchDesigner, YouTube</paragraph>
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