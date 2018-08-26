<template>
  <div>
    <video class="w100p" src="http://www.w3school.com.cn/i/movie.ogg" controls></video>

    <HeaderMore>详情</HeaderMore>

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
//H5头部
import SvgIcon from '../compsBase/SvgIcon'
import HeaderMore from '../compsHigh/HeaderMore'
export default {
  components: {
    SvgIcon,
    HeaderMore
  }
}
</script>
<style lang="scss">
</style>
