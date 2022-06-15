<template>
    <div class="works">
        <div class="content-area">
            <ttlTxt>墨汁の抽象化＜TouchDesignerを用いたノイズ表現＞</ttlTxt>
            <paragraph>複数のノイズが重なり、水墨画のように表現されたオブジェクトが徐々に単純化され、等高線で描かれた地図のようなオブジェクトに変化していく。<br>TouchDesignerを用いてノイズの変化と墨汁の抽象化を表現した。</paragraph>
            <contentImage
                :src="require(`~/assets/img/works/1.jpg`)"
            ></contentImage>
             <contentImage
                :src="require(`~/assets/img/other/td_noise.jpg`)"
            ></contentImage>
             <iframe src="https://www.youtube.com/embed/K_wJTB3JFeU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
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