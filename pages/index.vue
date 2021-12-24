<template>
  <div class="main">
    <commonHeader></commonHeader>
    <samples></samples>

    <div class="works">
      <div class="inner">
        <div class="container">
          <worksimg
          v-for='(data,index) in worksData'
          :key='data.title'
          :src="require(`~/assets/img/${index+1}.png`)"
          :linkPath='`work${index+1}`'
      ></worksimg>
        </div>
      </div>
    </div>
    
  </div>
</template>

<script>
import worksimg from '../components/worksimg.vue'
export default {
  components: { worksimg },
  name: 'IndexPage',
  data:()=>{
    return {
      worksData:[
        {title:'sample1'},
        {title:'sample1'},
        {title:'sample1'},
        {title:'sample1'},
        {title:'sample1'},
        {title:'sample1'}
      ]
    }    
  }
}
</script>

<style lang="scss">
.main {
  width: 100%;
  overflow: hidden;
  .works {
    padding: 68px 0;
    .inner {
        .container {
            margin: 0 auto;
            text-align: center;
            flex-wrap: wrap;
            display: flex;
            align-content: flex-start;
            justify-content: center;
        }
    }
}
}

@include mobile {
  
}

</style>
