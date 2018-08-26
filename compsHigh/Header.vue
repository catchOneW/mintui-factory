<template>
    <div>
        <div class="fxt ai bg-b color-w h90">
            <div class="fx1">
                <SvgIcon name="back"></SvgIcon>
            </div>
            <div class="fx1 tac fs35">
                <slot></slot>
            </div>
            <div class="fx1">
                <slot name="r"></slot>
            </div>
        </div>
        <div class="h90"></div>
    </div>
</template>
<script>
//H5头部
import SvgIcon from '../compsBase/SvgIcon'
export default {
  components: {
    SvgIcon
  }
}
</script>
<style lang="scss">
</style>
