<template>
    <div class="pd30">

        <div class="bdb">
            <div>人民医院</div>
            <img class="w100p mt30" src="../img/yiliao.png" alt="">
            <div class="pdtb30 df">
                <div class="tag">手机取号</div>
                <div class="tag">住院服务</div>
            </div>
        </div>
        <div class="df">
            <div class="fs0">
                <div class="pdt20">类别:</div>
                <div class="pdt20">性质:</div>
                <div class="pdt20">网址:</div>
                <div class="pdt20">联系电话:</div>
                <div class="pdt20">联系地址:</div>
            </div>
            <div class="ml30">
                <div class="pdt20">医院</div>
                <div class="pdt20">三甲</div>
                <div class="pdt20">www.szdpyy.com</div>
                <div class="pdt20">0755-33207898</div>
                <div class="line2 pdt20">xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</div>
            </div>

        </div>

        <HeaderMore>窗口简介</HeaderMore>

        <div class="ti2">
            xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
        </div>

        <div>
            <div class="fxb df h90 bg-w jcsa">
                <div class="ai-jc">
                    <SvgIcon name="zan1"></SvgIcon>
                    <span>0</span>
                </div>
                <div class="ai-jc">
                    <SvgIcon name="zan2"></SvgIcon>
                    <span>已搜藏</span>
                </div>
                <div class="ai-jc">
                    <SvgIcon name="share"></SvgIcon>
                    <span>分享</span>
                </div>
            </div>
            <div class="h90"></div>
        </div>
    </div>
</template>
<script>
//各种资讯列表
import SvgIcon from '../compsBase/SvgIcon'
import HeaderMore from '../compsHigh/HeaderMore'

export default {
  props: {
    arr: Array
  },
  components: {
    SvgIcon,
    HeaderMore
  },
  data() {
    return {
      arr2: {
        text:
          '111111111111111111111111111111111111111111111111111111111111111111111',
        types: [
          { name: '医疗场所2', icon: 'xuexiao' },
          { name: '医疗场所2', icon: 'xuexiao' }
        ],
        tags: ['三甲医院', '住院服务'],
        distance: '12.3km'
      }
    }
  }
}
</script>
<style lang="scss" scoped>
</style>
