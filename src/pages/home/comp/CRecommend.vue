<template>
  <div class="Recommend">
    <div v-for="item in myData" class="rec">
      <a :href="item.link"></a>
      <img :src="item.image" alt="">
      <div>{{item.title}}</div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'CRecommend',
    props: {
      myData: {
        type: Array,
        default() {
          return []
        }
      }
    }
  }
</script>

<style>
.Recommend{
  display: flex;
  padding: 5px 0px 15px 0px;
  border-bottom: 6px solid #EEE;
  text-align: center;
}
.rec{
  flex: 1;
}
.rec img{
  width: 65px;
  height: 65px;
}
</style>
