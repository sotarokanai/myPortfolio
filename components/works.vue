<template>
    <div class="works">
        <div class="container">
            <div class="container">
                <worksimg
                v-for='(data,index) in worksData'
                :key='data.title'
                :src="require(`~/assets/img/${index+1}.jpg`)"
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
        {title:'effectron - iOS App'},
        {title:'平塚サンダーバードちゃん - Music Video'},
        {title:'sommeil someil - Music Video'},
        {title:'霊障 - Book cover'},
        {title:'しずくだうみ - Music Video'},
        {title:'LED Vision'},
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