<template>
    <div class="works">
        <div class="content-area">
            <ttlTxt>LED Vision</ttlTxt>
            <paragraph>visual Effect</paragraph>
            <contentImage
            :src="require(`~/assets/img/other/led_l.jpg`)"        
            ></contentImage>
            <ttlTxt>tool</ttlTxt>
            <paragraph>TouchDesiner</paragraph>
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