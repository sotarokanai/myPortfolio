<template>
    <div class="info">
        <div class="content-area">
            <!-- <ttlTxt f_size="64px">inu</ttlTxt> -->
            <ttlTxt>profile</ttlTxt>
            <paragraph>kazuma kanai<br>visual effect / mobile app dev</paragraph>
            <ttlTxt>contact</ttlTxt>
            <paragraph>im@kazumakanai.com<br><a href="https://twitter.com/YYG_NT_LAB" style="text-decoration: underline;">Twitter</a></paragraph>
            <contentImage
                default_size="800px"
                :src="require(`~/assets/img/portrate.jpg`)"
            ></contentImage>
            <ttlTxt>tool</ttlTxt>
            <paragraph>touchdesigner, blender, unity, processingとか</paragraph>
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