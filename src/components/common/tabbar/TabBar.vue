<template>
  <div id="TabBar">
    <slot></slot>
  </div>
</template>

<script>
  export default {
    name: 'TabBar'
  }
</script>

<style>
#TabBar{
  display: flex;
  position: absolute;
  left: 0px;
  right: 0px;
  bottom: 0px;
  text-align: center;
}
</style>
