<template>
    <div class="article_detail">
        <div class="content-area">
            <!-- <ttlTxt f_size="64px">inu</ttlTxt> -->
            <ttlTxt>このページ使うかな</ttlTxt>
            <paragraph>作ったはいいけど書かないよなぁ</paragraph>
            <ttlTxt>マンモス</ttlTxt>
            <paragraph>うれぴい</paragraph>
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
.article_detail {
    width: 100%;
    overflow: hidden;
    .content-area {
        padding-top: 38px;
        width: 1144px;
        margin: 0 auto;
    }
}

@include mobile {
    .article_detail {
        .content-area {
            width: v(680);
            padding-top: v(38);
        }
    }
}
</style>