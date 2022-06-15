<template>
    <div class="works">
        <div class="content-area">
            <ttlTxt>name card</ttlTxt>
            <paragraph>デザインした名刺をAxiDrawを用いて印刷を行なった。</paragraph>
            <contentImage
            :src="require(`~/assets/img/other/DSC01990.jpg`)"        
            ></contentImage>
            <contentImage
            :src="require(`~/assets/img/other/DSC01972.jpg`)"        
            ></contentImage>
            <contentImage
            :src="require(`~/assets/img/other/namecard2.png`)"        
            ></contentImage>
            <ttlTxt>tool</ttlTxt>
            <paragraph>AxiDraw, Adobe Illustrator</paragraph>
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