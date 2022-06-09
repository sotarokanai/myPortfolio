<template>
    <div class="works">
        <div class="content-area">
            <ttlTxt>自己紹介</ttlTxt>
            <paragraph>planning, direction, visual Effect, design<br><a href="https://apps.apple.com/jp/app/effectron/id1526438768">download</a></paragraph>
            <contentImage
                :src="require(`~/assets/img/works/1.jpg`)"
            ></contentImage>
            <!-- srcの部分変えれば動画を埋め込めるで -->
            <iframe src="https://www.youtube.com/embed/zVonK6b82J8" title="YouTube video player" frameborder="0" allow=" autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" ></iframe>
            <ttlTxt>tool</ttlTxt>
            <paragraph>unity, ARFoundation</paragraph>
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