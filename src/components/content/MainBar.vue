<template>
  <TabBar>
    <TabBarItem>
      <div slot="text">Home</div>
    </TabBarItem>
    <TabBarItem>
      <div slot="text">Category</div>
    </TabBarItem>
    <TabBarItem>
      <div slot="text">Cart</div>
    </TabBarItem>
    <TabBarItem>
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
