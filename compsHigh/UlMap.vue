<template>
    <ul class="">
        <li class="ai pdlr30" v-for="(item,index) in arr2" :key="index">
            <SvgIcon class="mr30" name="position"></SvgIcon>
            <div class="fx1 ai bdb pdtb30">
                <div class="fx1">
                    <div class="line1" v-text="item.text"></div>
                    <div class="line1" v-text="item.address"></div>
                </div>
                <SvgIcon class="ml30 icon1" name="cc-arrow-left"></SvgIcon>
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
          address:
            '地址:111111111111111111111111111111111111111111111111111111111'
        },
        {
          text: '固戍地铁站',
          address: '地址:深圳市宝安区固戍地铁站'
        }
      ]
    }
  }
}
</script>
<style lang="scss" scoped>
.icon1 {
    transform: rotateZ(45deg)
}
</style>
