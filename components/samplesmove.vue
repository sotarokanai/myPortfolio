<template>
  <div id="app">
    <dashboard :id="'dashExample'">
      <dash-layout v-for="layout in dlayouts" v-bind="layout" :debug="false" :key="layout.breakpoint">
          {{layout.breakpoint}}
          
        <dash-item v-for="item in layout.items" v-bind.sync="item" :key="item.id">
          <!-- <div class="content" :background="url(item.gaga)"></div> -->
          <a class="box" href="#">
            <div class="content"  :style="{'background':`url(${item.ga}) center no-repeat`}">
              
              </div>
              <p>{{item.contentTtl}}</p>            
            </a>
          <!-- <img :src="item.ga" alt="" :width="item.gawidth" :height="item.gaheight"> -->
        </dash-item>
      </dash-layout>
    </dashboard>
  </div>
</template>

<script>
import { Dashboard, DashLayout, DashItem } from "vue-responsive-dash";

export default {
  name: "App",
  components: {
    Dashboard,
    DashLayout,
    DashItem
  },
  data() {
    return {
      dlayouts: [
        {
          breakpoint: "lg",
          breakpointWidth: 1200,
          numberOfCols: 10,
          items: [
            { id: "1", x: 0, y: 0, width: 4, height: 4, ga: require("~/assets/img/works/1.jpg"), contentTtl: "いぬのなまえ"},
            { id: "2", x: 4, y: 0, width: 2, height: 2 },
            { id: "3", x: 6, y: 0, width: 2, height: 2 },
            { id: "4", x: 8, y: 0, width: 2, height: 2 },
            { id: "5", x: 4, y: 2, width: 2, height: 2 },
            { id: "6", x: 6, y: 2, width: 2, height: 2 },
            { id: "7", x: 8, y: 2, width: 2, height: 2 },
          ]
        },
      ]
    };
  }
};
</script>

<style lang="scss">
.box {
  position: relative;
  .content {
    height: 100%;
    width: 100%;
    border: 1px solid $black;
    background-size: cover !important;
  }
  p {
      font-weight: bold;
      width: 100%;
      color: #fff;
      margin-top: -100px;
    }
}


.content:hover {
  filter: brightness(0.4);
}
</style>