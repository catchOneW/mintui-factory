<template>
  <div class="fs28">
    <Header>医疗卫生</Header>
    <!-- <div class="h338">
      <img src="./img/eduBanner.png" alt="" class="wh100p">
    </div> -->
    <!-- <UlMenu></UlMenu> -->
    <!-- <UlNews></UlNews> -->
    <!-- <HeaderMore></HeaderMore> -->
    <!-- <UlInfo></UlInfo> -->
    <!-- <UlYiliao></UlYiliao> -->
    <!-- <UlMap></UlMap> -->
    <!-- <YiliaoDetail></YiliaoDetail> -->
    <!-- <UlVideo></UlVideo> -->
    <!-- <VideoDetail></VideoDetail> -->
    <MapPage></MapPage>
  </div>
</template>
<script>
import './js/hotcss.js'
import './js/font.js'
//
import Header from './compsHigh/Header'
import HeaderMore from './compsHigh/HeaderMore'
import UlMenu from './compsHigh/UlMenu'
import UlNews from './compsHigh/UlNews'
import UlInfo from './compsHigh/UlInfo'
import UlYiliao from './compsHigh/UlYiliao'
import UlMap from './compsHigh/UlMap'
import UlVideo from './compsHigh/UlVideo'
import VideoDetail from './compsHigh/VideoDetail'
//
import YiliaoDetail from './page/YiliaoDetail'
import MapPage from './page/MapPage'

export default {
  components: {
    Header,
    UlMenu,
    UlNews,
    HeaderMore,
    UlInfo,
    UlYiliao,
    UlMap,
    YiliaoDetail,
    MapPage,
    UlVideo,
    VideoDetail
  },
  data() {
    return {}
  }
}
</script>
<style lang="scss">
@import './css/index.scss';
.tag {
  border: 1px solid #018ee1;
  color: #018ee1;
  @extend .pdlr10;
  @extend .mr20;
}
</style>
