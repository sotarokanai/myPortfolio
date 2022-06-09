<template>
    <div class="info">
        <div class="content-area">
            <!-- <ttlTxt f_size="64px">inu</ttlTxt> -->
            <ttlTxt>ttlTxtでかこうとタイトルになるで</ttlTxt>
            <paragraph>paragraphで書こうと本文サイズ<br>これ改行。</paragraph>
            <ttlTxt>contact</ttlTxt>
            <paragraph>im@kazumakanai.com<br>こんな感じでaで囲うとリンク<a href="https://twitter.com/" style="text-decoration: underline;">Twitter</a></paragraph>
            <!-- default_size="800px"ここでサイズ指定できる
            srcの中に好きな画像入れて -->
            <contentImage
                default_size="800px"
                :src="require(`~/assets/img/portrate.jpg`)"
            ></contentImage>
            <ttlTxt>tool</ttlTxt>
            <paragraph>example, example, example</paragraph>
        </div>
    </div>
</template>

<script>
import LergeTxt from '../../components/ttlTxt.vue'
export default {
    // data:() =>{
    //     return {
    //         contentImageData:[
    //             {contentimg}
    //         ]
    //     } 
    // }
   
}
</script>

<style lang="scss">
.info {
    width: 100%;
    overflow: hidden;
    .content-area {
        padding-top: 38px;
        width: 1144px;
        margin: 0 auto;
    }
}

@include mobile {
    .info {
        .content-area {
            width: v(680);
            padding-top: v(38);
        }
    }
}
</style>