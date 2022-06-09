<template>
    <div class="info">
        <div class="content-area">
            <ttlTxt>profile</ttlTxt>
            <paragraph>名前: 金井 奏太朗　カナイ ソウタロウ<br>出身: 群馬<br>年齢: 20<br>学校: 獨協大学 経済学部経済学科 在籍中<br>　　&nbsp;&nbsp;桑沢デザイン研究所 専攻デザイン科 ビジュアルデザイン専攻 在籍中<br>趣味: 散歩<br>愛犬: <a href="https://www.instagram.com/mamimi_inu/">まみみ</a></paragraph>
             <ttlTxt>tool</ttlTxt>
            <paragraph>Touch Designer, AxiDraw, Adobe: Illustrator Photoshop, ファイバーレーザーマーカー（光響製）,Nuxt.js</paragraph>
            <!-- default_size="800px"ここでサイズ指定できる
            srcの中に好きな画像入れて -->
            <contentImage
                default_size="800px"
                :src="require(`~/assets/img/info/portrate.jpg`)"
            ></contentImage>
            <ttlTxt>contact</ttlTxt>
            <paragraph>sotarokanai@gmail.com<br><a href="https://www.instagram.com/sotarokanai/" style="text-decoration: underline;">Instagram</a></paragraph>
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