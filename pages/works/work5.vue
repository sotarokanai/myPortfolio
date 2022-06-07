<template>
    <div class="works">
        <div class="content-area">
            <ttlTxt>しずくだうみ - Music Video</ttlTxt>
            <paragraph>direction, shootiong, editting</paragraph>
            <iframe src="https://www.youtube.com/embed/EyRGE-lPS_g" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            <ttlTxt>tool</ttlTxt>
            <paragraph>Premiere Pro, pen</paragraph>
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