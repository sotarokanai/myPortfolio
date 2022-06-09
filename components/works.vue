<template>
    <div class="works">
        <div class="container">
            <div class="container">
                <!-- assetsの中から1,2,3.jpgの順で読み込むようなっとるで -->
                <worksimg
                v-for='(data,index) in worksData'
                :key='data.title'
                :src="require(`~/assets/img/works/${index+1}.jpg`)"
                :linkPath='`works/work${index+1}`'
                :worksTtl='data.title'
                ></worksimg>
            </div>
        </div>
    </div>
</template>

<script>
import Works from '../components/works.vue'
import worksimg from '../components/worksimg.vue'
export default {
  components: { worksimg, Works },
  name: 'IndexPage',
  data:()=>{
    return {
      worksData:[
        // ページ増やすときはここにタイトル追加。works/works1,2,3.vueとassets/imgに1,2,3.jpgの追加も忘れずに
        {title:'猫さん'},
        {title:'順次タイトル追加2'},
        {title:'順次タイトル追加3'},
        {title:'順次タイトル追加4'},
        {title:'順次タイトル追加5'},
        {title:'順次タイトル追加6'},
        {title:'順次タイトル追加7'},
      ]
    }    
  }
}
</script>

<style lang="scss">
.works {
    .container {
        flex-wrap: wrap;
        display: flex;
        justify-content: space-between;
        width: 1144px;
        margin: 0 auto;
    }
}

@include mobile {
    .works {
    .container {
        width: v(680);
    }
}
}


</style>