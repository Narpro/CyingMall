<template>
  <Swiper>
    <SwiperItem v-for="item in myData">
      <a :href="item.link">
        <img :src="item.image" alt="">
      </a>
    </SwiperItem>
  </Swiper>
</template>

<script>
import {Swiper, SwiperItem} from '@/components/common/swiper'
export default {
  name: 'CSwiper',
  props: {
    myData: {
      type: Array,
      default() {
        return []
      }
    }
  },
  components: {
    Swiper,
    SwiperItem
  }
}
</script>

<style>

</style>
