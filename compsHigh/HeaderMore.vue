<template>
    <div class="ai bdb pd30">
        <div class="fs28 ai">
            <SvgIcon name="book"></SvgIcon>
            <div class="ml20">
                <slot>医疗咨询</slot>
            </div>
        </div>
        <div class="mla tar">
            更多>>
        </div>
    </div>
</template>
<script>
//查看更多 头部
import SvgIcon from '../compsBase/SvgIcon'
export default {
  components: {
    SvgIcon
  }
}
</script>
<style lang="scss">
</style>
