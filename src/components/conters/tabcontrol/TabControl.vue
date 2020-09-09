<template>
  <div class="home-control">
    <div v-for="(item,index) in ctitles">
      <span :class="{active:index===currentIndex}">{{item}}</span>
    </div>
  </div>
</template>

<script>
  export default {
    name: "TabControl",
    props:{
      ctitles:{
        type:Array,
        default(){
          return []
        }
      }
    },
    data(){
      return {
        currentIndex:0
      }
    }
  }
</script>

<style scoped>
  .active{
    color: var(--color-high-text);
    border-bottom: 4px solid var(--color-tint);
  }
</style>
