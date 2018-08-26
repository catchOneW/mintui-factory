<template>
    <ul class="">
        <li class="df pd30 bdb" v-for="(item,index) in arr2" :key="index">
            <div class="fx1 pdr40 ffc">
                <div class="line2" v-text="item.text"></div>
                <div class="mta" v-text="item.time"></div>
            </div>
            <div class="mla w230 h148">
                <img class="wh100p" :src="item.img" alt="">
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
          time: '2018-06-24',
          img:
            'https://news.91160.com/uploads/allimg/180809/33-1PP91146110-L.jpg',
        },
        {
          text:
            '111111111111111111111111111111111111111111111111111111111111111111111',
          time: '2018-06-24',
          img:
            'https://news.91160.com/uploads/allimg/180809/33-1PP91146110-L.jpg',
        },
      ]
    }
  }
}
</script>
<style lang="scss" scoped>

</style>
