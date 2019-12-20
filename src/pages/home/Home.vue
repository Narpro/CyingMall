<template>
  <div id="Home">
    <NavBar>
      <div slot="c-slot">Shopping Mall</div>
    </NavBar>
    <CSwper :myData="banner"/>
    <CRecom :myData="recommend"/>
  </div>
</template>

<script>

import NavBar from '@/components/common/navbar/NavBar'
import CSwper from './comp/CSwiper'
import CRecom from './comp/CRecommend'

import {getHomeMultidata} from '@/network/home'

export default {
  name: 'Home',
  data(){
    return {
      banner: [],
      recommend: []
    }
  },
  components: {
    NavBar,
    CSwper,
    CRecom
  },
  created(){
    getHomeMultidata().then(res => {
      this.banner = res.data.banner.list;
      this.recommend = res.data.recommend.list;
    })
  }
}
</script>

<style>

</style>
