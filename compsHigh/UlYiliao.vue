<template>
  <ul class="pdlr30">
    <li class="pdtb30 bdb" v-for="(item,index) in arr2" :key="index">
      <div class="line1" v-text="item.text"></div>
      <div class="df pdtb10">
        <div class="ai" v-for="(t,i) in item.types" :key="i">
          <SvgIcon :name="t.icon"></SvgIcon>
          <div class="mr20" v-text="t.name"></div>
        </div>
        <div class="mla" v-text="item.distance"></div>
      </div>
      <div class="df">
        <div v-for="(tg,j) in item.tags" :key="j">
          <div class="tag" v-text="tg"></div>
        </div>
      </div>
    </li>
  </ul>
</template>
<script>
//各种资讯列表
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
        {
          text:
            '111111111111111111111111111111111111111111111111111111111111111111111',
          types: [
            { name: '医疗场所2', icon: 'xuexiao' },
            { name: '医疗场所2', icon: 'xuexiao' }
          ],
          tags: ['三甲医院', '住院服务'],
          distance: '12.3km'
        },
        {
          text:
            '111111111111111111111111111111111111111111111111111111111111111111111',
          types: [
            { name: '医疗场所2', icon: 'xuexiao' },
            { name: '医疗场所2', icon: 'xuexiao' }
          ],
          tags: ['三甲医院', '住院服务'],
          distance: '12.3km'
        },
        {
          text:
            '111111111111111111111111111111111111111111111111111111111111111111111',
          types: [
            { name: '医疗场所2', icon: 'xuexiao' },
            { name: '医疗场所2', icon: 'xuexiao' }
          ],
          tags: ['三甲医院', '住院服务'],
          distance: '12.3km'
        }
      ]
    }
  }
}
</script>
<style lang="scss" scoped>

</style>
