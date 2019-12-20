<template>
  <TabBar>
    <TabBarItem path='/home'>
      <Icon slot="icon-active" type="ios-home" />
      <Icon slot="icon" type="ios-home-outline" />
      <div slot="text">Home</div>
    </TabBarItem>
    <TabBarItem path='/category'>
      <Icon slot="icon-active" type="ios-list-box" />
      <Icon slot="icon" type="ios-list-box-outline" />
      <div slot="text">Category</div>
    </TabBarItem>
    <TabBarItem path='/cart'>
      <Icon slot="icon-active" type="ios-cart" />
      <Icon slot="icon" type="ios-cart-outline" />
      <div slot="text">Cart</div>
    </TabBarItem>
    <TabBarItem path='/profile'>
      <Icon slot="icon-active" type="ios-person" />
      <Icon slot="icon" type="ios-person-outline" />
      <div slot="text">Profile</div>
    </TabBarItem>
  </TabBar>
</template>

<script>
  import TabBar from '../common/tabbar/TabBar'
  import TabBarItem from '../common/tabbar/TabBarItem'
  export default {
    name: 'MainBar',
    components: {
      TabBar,
      TabBarItem
    }
  }
</script>

<style>

</style>
