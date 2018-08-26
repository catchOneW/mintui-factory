<template>
  <div id="mapPage" class="por l0 r0 t0 b0">
    <el-amap vid="amap" :zoom="12" :plugin="plugin">
      <el-amap-marker v-for="(marker,index) in markers" :key="index" :position="marker"></el-amap-marker>
    </el-amap>
    <el-amap-search-box class="search-box fs30" :search-option="searchOption" :on-search-result="onSearchResult"></el-amap-search-box>
    <div class="zoomBtn poa ffc bg-w">
      <SvgIcon name="add"></SvgIcon>
      <SvgIcon name="minus"></SvgIcon>
    </div>
  </div>
</template>
<script>
//H5头部
import Vue from 'vue'
import SvgIcon from '../compsBase/SvgIcon'
import VueAMap from 'vue-amap'
Vue.use(VueAMap)
VueAMap.initAMapApiLoader({
  // 高德的key
  key: '0424c78c3ea118ec419c31eab8154562',
  // 插件集合
  plugin: [
    'AMap.Autocomplete',
    'AMap.PlaceSearch',
    'AMap.Scale',
    'AMap.OverView',
    'AMap.ToolBar',
    'AMap.MapType',
    'AMap.PolyEditor',
    'AMap.CircleEditor'
  ],
  // 高德 sdk 版本，默认为 1.4.4
  v: '1.4.4'
})
export default {
  components: {
    SvgIcon,
    VueAMap
  },
  mounted() {},
  data() {
    return {
      markers: [
        [121.59996, 31.197646],
        [121.40018, 31.197622],
        [121.69991, 31.207649]
      ],
      searchOption: {},
      mapCenter: [121.59996, 31.197646],

      plugin: [
        {
          pName: 'Scale',
          events: {
            init(instance) {
              console.log(instance)
            }
          }
        }
      ]
    }
  },
  methods: {
    addMarker: function() {
      let lng = 121.5 + Math.round(Math.random() * 1000) / 10000
      let lat = 31.197646 + Math.round(Math.random() * 500) / 10000
      this.markers.push([lng, lat])
    },
    onSearchResult(pois) {
      let latSum = 0
      let lngSum = 0
      if (pois.length > 0) {
        pois.forEach(poi => {
          let { lng, lat } = poi
          lngSum += lng
          latSum += lat
          this.markers.push([poi.lng, poi.lat])
        })
        let center = {
          lng: lngSum / pois.length,
          lat: latSum / pois.length
        }
        this.mapCenter = [center.lng, center.lat]
      }
      console.log(1111111);
      
    }
  }
}
</script>
<style lang="scss">
.zoomBtn {
  left: 0.3rem;
  top: 8rem;
}
#mapPage {
  .search-box {
    position: absolute;
    left: 50%;
    top: 2rem;
    transform: translate(-50%, -50%);
    width: 90%;
    input {
      height: 0.9rem;
      font-size: 0.28rem
    }
  }
}
</style>


