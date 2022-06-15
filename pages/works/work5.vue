<template>
    <div class="works">
        <div class="content-area">
            <ttlTxt>Laser Marking</ttlTxt>
            <paragraph>製作した土版に、TouchDesignerで生成した複数の模様をファイバーレーザーマーカーを用いて印刷した。</paragraph>
             <contentImage
            :src="require(`~/assets/img/other/laser.jpg`)"
            ></contentImage>
            <contentImage
            :src="require(`~/assets/img/other/laser2.jpg`)"
            ></contentImage>
            <contentImage
            :src="require(`~/assets/img/other/line3.png`)"
            ></contentImage>
            <ttlTxt>tool</ttlTxt>
            <paragraph>ファイバーレーザーマーカー（光響製）, ヤコのオーブン陶土 TouchDesigner</paragraph>
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