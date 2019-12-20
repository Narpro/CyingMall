<template>
  <div class="TabBarItem">
    <div>
      <slot name="icon-active"></slot>
    </div>
    <div>
      <slot name="icon"></slot>
    </div>
    <div>
      <slot name="text"></slot>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'TabBarItem'
  }
</script>

<style>
.TabBarItem{
  flex: 1;
}
</style>
