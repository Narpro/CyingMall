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
  height: 50px;
  text-align: center;
  background: #EEE;
}
</style>
