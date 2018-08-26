<template>
    <ul class="ffr">
        <li class="col4 ai-jc ffc pdt40 pdb36 bdr bdb" v-for="(item,index) in arr2" :key="index">
            <SvgIcon :name="item.icon"></SvgIcon>
            <div class="mt20" v-text="item.name"></div>
        </li>
    </ul>
</template>
<script>
//2列菜单
import SvgIcon from '../compsBase/SvgIcon'
export default {
  props: {
    arr: Array
  },
  components: {
    SvgIcon
  },
  data() {
    return {
      arr2: [
        { name: '医疗场所2', icon: 'xuexiao' },
        { name: '计生窗口', icon: 'videoa' },
        { name: '医疗视频', icon: 'building_' },
        { name: '医疗地图', icon: 'book' },
        { name: '医疗指南', icon: 'jiaoyu' }
      ]
    }
  }
}
</script>
<style lang="scss" scoped>
</style>
