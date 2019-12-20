<template>
  <div class="NavBar">
    <div class="right">
      <slot name="r-slot"></slot>
    </div>
    <div class="center">
      <slot name="c-slot"></slot>
    </div>
    <div class="left">
      <slot name="l-slot"></slot>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'NavBar',
    props: {
      navColor: {
        type: String,
        default: 'rgb(255,141,148)'
      }
    },
    mounted(){
      document.getElementsByClassName('NavBar')[0].style.background = this.navColor;
    }
  }
</script>

<style>
.NavBar{
  height: 45px;
  line-height: 45px;
  display: flex;
  text-align: center;
  color: white;
}
.right, .left{
  width: 50px;
}
.center{
  flex: 1;
}
</style>
