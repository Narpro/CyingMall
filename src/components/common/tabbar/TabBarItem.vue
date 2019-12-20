<template>
  <div class="TabBarItem" @click="clicked">
    <div v-if="isActive">
      <slot name="icon-active"></slot>
    </div>
    <div v-else>
      <slot name="icon"></slot>
    </div>
    <div>
      <slot name="text"></slot>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'TabBarItem',
    props: {
      path: String
    },
    methods: {
      clicked(){
        this.$router.replace(this.path);
      }
    },
    computed: {
      isActive(){
        return this.$route.path === this.path;
      }
    }
  }
</script>

<style>
.TabBarItem{
  flex: 1;
}
.ivu-icon{
  font-size: 20px;
}
</style>
