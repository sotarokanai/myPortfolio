<template>
    <div class="works">
        <div class="content-area">
            <ttlTxt>平塚サンダーバードちゃん - Music Video</ttlTxt>
            <paragraph>direction, shootiong, editing</paragraph>
            <!-- <contentImage
                :src="require(`~/assets/img/2.jpg`)"
            ></contentImage> -->
            <iframe src="https://www.youtube.com/embed/Cgv8jWykfaw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            <ttlTxt>tool</ttlTxt>
            <paragraph>AfterEffects, hydra, youtube</paragraph>
            <ttlTxt>publication</ttlTxt>
            <paragraph><a href="https://japanese.engadget.com/effectron-dev-023013942.html">iOSアプリ開発者に訊く：LiDARで空間を演出するEffectron</a></paragraph>
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